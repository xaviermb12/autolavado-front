<template>
  <div class="title">
    <div>
      <vs-input
        v-model="Usuario"
        label="Usuario"
        placeholder="Escriba su Usuario"
      />
    </div>
    <div>
      <vs-input
        v-model="Contraseña"
        type="password"
        label="Contraseña"
        placeholder="Escriba su Contraseña"
      />
    </div>
    <div>
      <vs-button :active="active == 0" @click="active = 0">Ingresar</vs-button>
    </div>
    <div class="links">
      <nuxt-link to="/Login-RecuperarContraseña"
        >Recuperar Contraseña</nuxt-link
      >
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    Usuario: '',
    Contraseña: ''
  })
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 30px;
  color: #35495e;
  letter-spacing: 1px;
  text-transform: capitalize;
  margin: 5% auto;
  margin-left: 15%;
}

.subtitle {
  font-weight: 300;
  font-size: 1.1rem;
  color: #526488;
  word-spacing: 2px;
  padding-bottom: 15px;
  max-width: 600px;
}

.subtitle a {
  font-weight: 500;
  color: inherit;
}

.links {
  padding-top: 15px;
  margin-bottom: 20px;
}

.content-logos {
  display: flex;
  align-items: center;
  justify-content: center;
  min-width: 500px;
}
.plus {
  font-size: 2.5rem;
  margin: 15px;
  color: #35495e;
}
.h3 {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-weight: 400;
  margin: 10px;
}

.vs-input {
  margin: 20px;
}
</style>
