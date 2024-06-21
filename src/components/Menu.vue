<template>
  <div id="menu">
    <img src="../assets/img/logo.png" alt="Logo" id="logo">
    <ul>
      <li><a href="#sobre">Sobre</a></li>
      <li><a href="#projetos">Projetos</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#contato">Contato</a></li>
    </ul>
  </div>
  <div id="cabecalho">
    <div class="container-esquerdo">
      <img src="../assets/img/me.png" alt="avatar" id="avatar">
    </div>
    <div class="apresentacao">
      <div class="texto-apresentacao">
        <h2>Oi, eu sou a Lorrayne Antonielle!</h2>
        <p>
          Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
        </p>
      </div>
    </div>
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
  background-color: transparent;
}

#menu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  float: right;
}

#menu ul li {
  float: left;
  justify-content: center;
  align-items: center;
}

#menu ul li a {
  display: block;
  color: #3d405b;
  text-align: center;
  padding: 20px 20px;
  text-decoration: none;
  font-size: 22px;
}

#menu ul li a:hover {
  font-size:20px;
}
#logo {
  float: left;
  padding: 10px;
  max-width: 100px;
  background-color: red;
}

#cabecalho {
  min-height: 600px;
  background-color: #f2cc8f;
  margin-top:-80px;
  display: flex;
  width: 100%;
}
.container-esquerdo{
  background-color: #3d405b;
  min-height: 600px;
  max-width: 30%;
  display: flex;
  justify-content: center;
}
#avatar {
  max-width: 350px;
  align-self: center;
  margin-left:100%;
  border-radius: 50%;
}
.apresentacao{
  justify-content: center;
  display:flex;
  min-width: 70%;
  align-items: center;
}
.apresentacao h2{
  align-items: center;
  font-size:33px;
}
.texto-apresentacao{
  max-width: 60%;
}
.texto-apresentacao p{
  font-size:18px;
}
</style>
