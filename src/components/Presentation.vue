<template>
    <div class="presentation__container">
        <div class="section">
            <div class="question">
            <h1 class="presentation un">C'est quoi un développeur ? 👀</h1>
            <h3 class="reponse" @click="seeResponse(0)">Réponse 📣</h3>
            </div>
            <article v-if="articles[0].switch">
                <h4>"En informatique, un développeur ou analyste programmeur est un informaticien qui réalise des logiciels et les met en œuvre à <br> l'aide de langages de programmation."- Wikipédia</h4>
            </article>
        </div>
        <div class="section">
            <div class="question">
                <h1 class="presentation deux">🤨 Mais concrètement, tu fais quoi ?</h1>
                <h3 class="reponse" @click="seeResponse(1)">Réponse 📣</h3>
            </div>
            <article v-if="articles[1].switch">
                <p class="note">* L'ensembles des termes sont définis, il suffit de cliquer dessus 😉</p>
                <h4>En quelque mots mon boulot c'est de <span><a target="_blank" href="https://www.youtube.com/watch?v=9OBnvpzb560&ab_channel=br95120">résoudre des problèmes</a></span>, plus ou moins complexes selon les projets. Je réalise essentiellement des sites Web ainsi que applications Web et Mobiles. J'interviens aussi bien sur le <span><a target="_blank" href="https://www.kicklox.com/blog-talent/developpeur-front-end">Front-end</a></span> que le <span><a target="_blank" href="https://www.clementine.jobs/fiches-metiers/metiers-techniques-du-web/developpeur-back-end/#:~:text=Le%20D%C3%A9veloppeur%20Back%2DEnd%20est,Il%20travaille%20dans%20l'ombre.">Back-end</a></span>, dans le jargon on appelle ça un developpeur <span><a target="_blank" href="https://hackernoon.com/drafts/j41mp32tc.png">Fullstack</a></span> ! 😎</h4>
            </article>
        </div>
        <div class="section">
            <div class="question">
                <h1 class="presentation trois">Tu aime ce que tu fais ? 🥰</h1>
                <h3 class="reponse" @click="seeResponse(2)">Réponse 📣</h3>
            </div>
            <article v-if="articles[2].switch">
                <p class="note">* L'ensembles des termes sont définis, il suffit de cliquer dessus 😉</p>
                <h4>Cela fait maintenant quelques années que je me suis plongé corps et âmes dans le milieu de la Programmation, j'ai développé une vrai passion pour ce métier et les différentes facettes qui le compose. </h4> 
                <h4> Formé chez <span><a target="_blank" href="https://ecole-webstart.com/?gclid=Cj0KCQjwo-aCBhC-ARIsAAkNQitf3xFa8M2Hdfmm3fjHEjBIZqkIZe5OmMExvG-3QXKt7qDRnau7eT0aAiDBEALw_wcB">Webstart</a></span>, j'y ai appris les bases de la programmation, mais aussi et surtout LA qualitée qui selon moi est primordiale chez un développeur, L'AUTODIDACTIE, la <span><a target="_blank" href="https://www.youtube.com/watch?v=q6VxDM8Wd-o&ab_channel=DealerdeMeme">DÉBROUILLARDISE</a></span>! J'ai donc parallèlement a l'école commencé a me former seul sur divers sujet (<span><a target="_blank" href="https://fr.wikipedia.org/wiki/Programmation_dynamique">Dynamic Programming</a></span>, <span><a target="_blank" href="https://www.python.org/about/apps/">Python</a></span>, <span><a target="_blank" href="https://www.apple.com/fr/swift/">Swift</a></span>, <span><a target="_blank" href="https://fr.wikipedia.org/wiki/Apprentissage_automatique">Machine Learning</a></span>, <span><a target="_blank" href="https://fr.reactjs.org/">React</a></span>), Google est un puit sans fond de connaissances et d'exemples pour progresser en tant que développeur.
                </h4>
            </article>
        </div>
        <div class="section">
            <div class="question">
                <h1 class="presentation quatre">🤔 C'est bien sympa tout ça, mais sur quels projets as tu travaillé ?</h1>
                <h3 class="reponse" @click="seeResponse(3)">Réponse 📣</h3>
            </div>
            <article v-if="articles[3].switch">
                <div class="projects">
                    <h4>Tout est là ! 👉</h4>
                    <a target="_blank" href="https://github.com/JessimH"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/91/Octicons-mark-github.svg/1024px-Octicons-mark-github.svg.png" alt=""></a>
                </div>
            </article>
        </div>
        <div class="section">
            <div class="question">
            <h1 class="presentation cinq">WAW ! Et tu pourrais hacker un compte Facebook pour moi ? 😈</h1>
                <h3 class="reponse" @click="seeResponse(4)">Réponse 📣</h3>
            </div>
            <article v-if="articles[4].switch">
                <p class="note">* L'ensembles des termes sont définis, il suffit de cliquer dessus 😉</p>
                <h4>NON! Mais tu peux trouver la marche à suivre <span><a target="_blank" href="https://www.youtube.com/watch?v=leeIukABB4k&ab_channel=ArmandMarolle">ici</a></span> 👈
                </h4>
            </article>
        </div>
    </div>
</template>
<script>
export default {
  name: 'Presentation',
  data() {
      return {
          articles: [
              {
              switch: false,
              id: 1,
            },
            {
              switch: false,
              id: 2,
            },
            {
              switch: false,
              id: 3,
            },
            {
              switch: false,
              id: 4,
            },
            {
              switch: false,
              id: 5,
            }
          ]
      }
  },
  methods: {
      seeResponse(id){
          for(let i = 0; i <= this.articles.length - 1; i++){
                this.articles[i].switch = false 
          }
          this.articles[id].switch = !this.articles[id].switch
      }
  }
}
</script>

<style lang="css" scoped>
.presentation__container{
    padding: 40px;
    text-align: left;
}
.presentation{
    padding: 20px;
    text-align: left;
}
h1{
    background-color: yellow;
    font-size: 1.5em;
    padding: 10px;
    max-width: fit-content;
    box-shadow: 11px 11px 0px 0px #2c3e50;

}
article{
    padding-left: 30px;
    padding-right: 30px;
    margin-top: 30px;
    margin-bottom: 50px;
}
article h4 span {
    color: #42b983;
}
article h4 span a {
    text-decoration: none;
    color: #42b983;
    transition: 0.1s ease;
}
article h4 span a:hover {
    text-decoration: none;
    color: red;
}

.projects{
    display: flex;
    flex-wrap: wrap;
    align-items: center;
}

img{
    margin-left: 10px;
    max-width: 40px;
}

.reponse{
    background: #42b983;
    max-width: fit-content;
    padding:10px;
    box-shadow: 9px 9px 0px 0px #2c3e50;
    cursor: pointer;
    transition:0.2s ease;
}

.reponse:hover{
    background: red;
    color: white;
    max-width: fit-content;
    padding:10px;
    box-shadow: 9px 9px 0px 0px #2c3e50;
    cursor: pointer;
    transform: scale(1.04);
}
.section{
    margin-bottom: 50px;
}

.un{ 
    background-color: #1E31C9;
    color: white;
}

.deux{
    background-color: #FB1E14;
    color: white;
}

.quatre{
    background-color: #42b983;
    color: white;
}

.cinq{
    background-color: #1E31C9;
    color: white;
}
</style>