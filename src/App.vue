<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <MenuPrincipal msg="apresentacao"/>
  <SoftHardSkills msg="skills" />
</template>

<script>
import MenuPrincipal from './components/Menu.vue'
import SoftHardSkills from './components/Skills.vue'

export default {
  name: 'App',
  components: {
    MenuPrincipal ,
    SoftHardSkills
  }
}
</script>

<style>
#app {
  font-family: "Kanit", sans-serif;
  text-align: center;
  color: #2c3e50;
  padding:0;
}
</style>
