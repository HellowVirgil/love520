<template>
  <div id="app">
    <Index text="Love" />
  </div>
</template>

<script>
import Index from './components/Index.vue'

export default {
  name: 'app',
  components: {
    Index
  }
}
</script>

<style>
body {
  width: 100%;
  height: 100%;
  margin: 0;
  padding: 0;
  background-color: #e41749;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
