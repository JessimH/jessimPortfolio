<template>
  <div>
      <div class="notFound">
        <div class="head">
            <h1 class="title"> 404 </h1>
        </div>
        <p>La page que vous cherchez n'existe pas! Désolé ! 🤨</p>
        <a class="button" href="/">Retourner a l'Accueil 👈 </a>
      </div>
    <Footer/>
  </div>
</template>

<script>
import Footer from '../components/Footer.vue'


  export default {
    name: 'page404',
    components: {
        Footer
    }
  }

</script>

<style scoped>
.notFound{
    height: 73.5vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background: url('https://media.giphy.com/media/kHU8W94VS329y/giphy-downsized-large.gif')
}
.head{
    width:100%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
}
p{
    font-size: 1.3em;
    background-color:#1E31C9;
    box-shadow: 9px 9px 0px 0px #2c3e50;
    padding: 10px;
    color: white;
}
.title{
    font-size: 10em;
    color: white;
    margin: 0;
    padding: 0;
}
img{
    max-width: 100%;
}
.button{
    font-weight: bold;
    font-size: 1.5em;
    background-color: yellow;
    box-shadow: 9px 9px 0px 0px #2c3e50;
    padding: 10px;
    max-width: fit-content;
    text-decoration: none;
    color: #2c3e50;
}
.button:hover{
    background-color: red;
    cursor: pointer;
    color: white;
}
</style>