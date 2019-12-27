<template>
  <section>
    <h1>fuga {{ id }}</h1>
    <nuxt-link to="/">戻る</nuxt-link>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  data() {
    return {
      ...this.$route.params
    }
  }
}
</script>
