<template xmlns:v-on="http://www.w3.org/1999/xhtml">
  <div id="app">
    <img src="./assets/logo.png" v-on:click="go">
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app',
  methods: {
    go: function () {
      this.$router.push('World')
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
