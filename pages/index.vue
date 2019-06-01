<template>
  <section class="container">
    <div>
      <h1 class="title">My first Nuxt app</h1>
      <nuxt-link to=" /users">Users</nuxt-link>
      <button @click="goToProducts">Go to products</button>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    goToProducts() {
      this.$router.push('/products')
    }
  }
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
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
</style>
