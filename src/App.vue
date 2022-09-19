<template>
  <div id="app">
    <ServerList />
    <ServerDetils />

  </div>
</template>

<script>

import ServerList from './components/server/ServersList.vue'
import ServerDetils from './components/server/ServerDetails.vue'

export default {
  name: 'App',
  components: {
    ServerList,
    ServerDetils 
    
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
