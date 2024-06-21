<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <MenuPrincipal msg="teste"/>
</template>

<script>
import MenuPrincipal from './components/Menu.vue'

export default {
  name: 'App',
  components: {
    MenuPrincipal 
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: red;
}
</style>
