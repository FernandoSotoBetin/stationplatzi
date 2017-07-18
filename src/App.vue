<template lang="pug">
  #app.container
      section
        div
          img(src="./assets/station_platzi.jpg")
        h1 Registro estación Platzi
        form
          .field.control
            label.label(for='nombre') Nombre
            input.inputs(type='text', name='nombre', placeholder='Fernando')
          .field.control
            label.label(for='apellido') Apellido
            input.inputs(type='text', name='apellido', placeholder='Soto')
          .field.control
            label.label(for='cargo') Cargo
            input.inputs(type='text', placeholder='Full Stack')
          .field.align
            input.button(v-on:click="enviar", type='button', value='ENVIAR')
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Hello',
      nombre: 'Fernando'
    }
  },

  methods: {
    enviar: function() {
      alert("Datos Enviados Satisfactoriamente");
    }
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Roboto:400,700');
@import './scss/main.scss';
</style>
