<template lang="html">
  <div class="container">
    <div class="title">
      <nuxt-link to="/">Home page</nuxt-link>
    </div>
    <div class="develop">
      <div v-if="toggle">
        <p>{{ msg }}</p>
      </div>
      <div class="linkURL">
        <p><a :href="url">Google Link</a></p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "hello!",
      toggle: true,
      url: 'https://google.com'
    }
  }
}
</script>

<style lang="css" scoped>
.container {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  margin: 0 auto;
  min-height: 100vh;
  max-width: 600px;
  font-size: 24px;
}
.title {
  font-weight: 300;
  font-size: 40px;
  color: #35495e;
  letter-spacing: 1px;
}
.links {
  padding-top: 15px;
}
</style>
