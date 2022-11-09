<template>
  <div>
    <h1>test first</h1>
    <form method="get" action="#" v-on:submit.prevent="onLoadUser">
      <input type="text" id="userId" v-model="userId">
      <button type="submit">Load User</button>
    </form>
    <nuxt-child></nuxt-child>
  </div>
</template>

<script>
export default {
  name: "users",
  data () {
    return {
      userId: 0
    }
  },
  methods: {
    onLoadUser() {
      this.$router.push('/users/' + this.userId)
    }
  }
}
</script>

<style scoped>

</style>
