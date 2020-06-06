<template>
  <div>
    <h1>{{ paquetes }}</h1>
  </div>
</template>

<script>
export default {
  computed: {
    paquetes() {
      return this.$store.state.admin.paquetes.data
    }
  },
  methods: {
    getPaquetes() {
      this.$store.dispatch('/admin/paquetes/getPaquetes')
    }
  }
}
</script>
