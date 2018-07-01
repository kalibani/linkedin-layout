<template>
  <div class="app">
    <app-body></app-body>
  </div>
</template>

<script>
import AppBody from './pages/AppBody'
export default {
  name: 'MainComponent',
  components: {
    AppBody
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
</style>
