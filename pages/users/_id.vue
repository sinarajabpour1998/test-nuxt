<template>
  <div>
    <br>
    test id:  {{ $route.params.id }}
    <br>
    <nuxt-link to="/users"><- Back</nuxt-link>
  </div>
</template>

<script>
export default {
  validate(data) {
    // check if it's an integer
    return /^\d+$/.test(data.params.id);
  }
}
</script>

<style scoped>

</style>
