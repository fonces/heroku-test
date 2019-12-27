<template>
  <section>
    <h1>index</h1>
    <nuxt-link to="/hoge">hoge</nuxt-link>
    <input
      v-model="fugaId"
      type="text">
    <nuxt-link :to="fugaLink">fuga</nuxt-link>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  data: () => ({ fugaId: '' }),
  computed: {
    fugaLink() {
      return `/fuga/${this.fugaId}`
    }
  }
}
</script>

<style scoped>
input {
  border: solid 1px gray;
}
</style>
