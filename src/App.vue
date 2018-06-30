<template>
  <div id="app">
    <app-navbar></app-navbar>
    <router-view/>
  </div>
</template>

<script>
import AppNavbar from '@/components/pages/AppNavbar'
export default {
  name: 'App',
  components: {
    AppNavbar
  }
}
</script>

<style>
body {
  background-color: #F5F5F5;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
