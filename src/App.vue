<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
import './static/lib/css/main.css'
export default {
  name: 'app'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  position:absolute;
  top:0;
  bottom:0;
  left:0;
  right:0;
}
</style>
