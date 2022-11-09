<template>
  <div>
    <h1 v-if="error.statusCode === 404">Page not found</h1>
    <h1 v-else>Oops ! something happened...</h1>
    <br>
    <nuxt-link to="/">Back</nuxt-link>
  </div>
</template>

<script>
export default {
  props: ["error"],
  name: "error"
}
</script>

<style scoped>

</style>
