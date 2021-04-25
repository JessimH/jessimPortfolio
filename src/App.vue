<template>
  <div id="nav">
    <h1 class="logo">J.</h1>
    <router-link to="/">Accueil</router-link>
    <router-link to="/about">CV</router-link>
  </div>
  <router-view/>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

#app {
  font-family: 'Poppins', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100vw;
  margin: 0;
  padding: 0;
}

#nav {
  background-color: white;
  padding-top: 20px;
  padding-bottom: 20px;
  padding-left: 30px;
  display:flex;
  justify-content: flex-start;
  align-items: center;
  position: sticky;
  top: 0;
}

#nav a {
  font-weight: bold;
  background-color: yellow;
  box-shadow: 5px 5px 0px 0px #2c3e50;
  padding: 10px;
  color: #2c3e50;
  text-decoration:none;
  transition: 0.2s ease;
  margin-left: 20px;
  margin-right: 20px;
}

#nav a:hover{
  transform: scale(1.04);
}

#nav a.router-link-exact-active {

  background-color: red;
  color: white;
}
#nav h1{
  margin: 0;
  font-size: 3em;
}
</style>
