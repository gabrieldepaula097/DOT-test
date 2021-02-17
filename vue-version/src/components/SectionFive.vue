<template>
  <div class="p-0 div-main-triangle h-30 center-flex">
    <b-form
      @submit="onSubmit"
      :class="{ 'h-66': !checkMobile, 'h-85': checkMobile }"
    >
      <div class="row" :class="{ 'm-0': checkMobile }">
        <div class="col-12">
          <b-form-group id="input-group-1">
            <b-form-input
              id="input-1"
              v-model="form.name"
              type="text"
              placeholder="*Nome: Informe seu nome"
              :state="nameState"
              aria-describedby="input-1-feedback"
              required
            ></b-form-input>
            <b-form-invalid-feedback id="input-live-feedback" class="text-left">
              Digite pelo menos 3 caracteres
            </b-form-invalid-feedback>
          </b-form-group>
        </div>
        <div class="col-12 col-lg-6">
          <b-form-group id="input-group-2">
            <b-form-input
              id="input-2"
              v-model="form.email"
              type="email"
              placeholder="*E-mail: Informe seu e-mail"
              required
            ></b-form-input>
          </b-form-group>
        </div>
        <div class="col-12 col-lg-6">
          <b-form-group id="input-group-3">
            <b-form-input
              id="input-3"
              v-model="form.phone"
              type="tel"
              placeholder="*Telefone: (__) _____-____"
              :formatter="formatter"
              required
            ></b-form-input>
          </b-form-group>
        </div>
        <div class="col-12">
          <b-form-group id="input-group-4">
            <b-form-textarea
              id="input-4"
              v-model="form.message"
              placeholder="*Mensagem: Escreva aqui"
              size="md"
              rows="5"
              :state="messageState"
              aria-describedby="input-2-feedback"
              required
            ></b-form-textarea>
            <b-form-invalid-feedback id="input-live-feedback" class="text-left">
              Digite pelo menos 20 caracteres
            </b-form-invalid-feedback>
          </b-form-group>
        </div>
        <div class="col-12">
          <b-button type="submit" variant="light" class="button-submit"
            >ENVIAR</b-button
          >
        </div>
      </div>
    </b-form>
  </div>
</template>

<script>
export default {
  props: ["checkMobile"],
  data() {
    return {
      form: {
        email: "",
        name: "",
        phone: "",
        message: ""
      }
    };
  },
  computed: {
    nameState() {
      return this.form.name.length > 2 ? true : false;
    },
    messageState() {
      return this.form.message.length > 20 ? true : false;
    }
  },
  methods: {
    onSubmit(event) {
      event.preventDefault();
      alert("Formulário validado:\n" + JSON.stringify(this.form));
    },
    formatter(value) {
      var x = null;
      if (value.length > 14) {
        x = value.replace(/\D/g, "").match(/(\d{0,2})(\d{0,5})(\d{0,4})/);
      } else if (value.length <= 14) {
        x = value.replace(/\D/g, "").match(/(\d{0,2})(\d{0,4})(\d{0,4})/);
      }

      return (value = !x[2]
        ? x[1]
        : "(" + x[1] + ") " + x[2] + (x[3] ? "-" + x[3] : ""));
    }
  }
};
</script>

<style lang="css">
.div-main-triangle {
  background: -webkit-gradient(
    linear,
    left top,
    right bottom,
    color-stop(50%, #707070),
    color-stop(50%, #434343)
  );
  background: -webkit-linear-gradient(top left, #707070 50%, #434343 50%);
  background: -o-linear-gradient(top left, #707070 50%, #434343 50%);
  background: linear-gradient(to bottom right, #707070 50%, #434343 50%);
}

.form-control {
  background-color: #bfbfbf !important;
}

.form-control:focus {
  outline: none !important;
  box-shadow: none !important;
  border-color: #bfbfbf !important;
}

.button-submit {
  width: 9rem;
  height: 3.5rem;
  font-weight: bold !important;
}
</style>
