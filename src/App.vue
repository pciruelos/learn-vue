<template>
  <div id="app">
    <Primer/>
  </div>
</template>

<script>
import Primer from './components/Primer.vue'

export default {
  name: 'App',
  components: {
    Primer
    
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
