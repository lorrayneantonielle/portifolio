<template>
  <div id="menu">
    <img src="logo.png" alt="Logo" id="logo">
    <ul>
      <li><a href="#sobre">Sobre</a></li>
      <li><a href="#projetos">Projetos</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#contato">Contato</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'MenuPrincipal',
  props: {
    msg: String
  }
}
</script>

<style scoped>
#menu {
  overflow: hidden;
  background-color: #333;
}

#menu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  float: right;
}

#menu ul li {
  float: left;
}

#menu ul li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

#menu ul li a:hover {
  background-color: #111;
}
#logo {
  float: left;
  padding: 10px;
}
</style>
