<template>
    <div class="card">
        <div class="card__profile">
            <img class="card__profileImage" src="https://media-exp1.licdn.com/dms/image/C4D03AQGKp9RWsjlFkw/profile-displayphoto-shrink_800_800/0/1617122696986?e=1625097600&v=beta&t=EH5bAvYc_VAZ7sLC5ytJ0tAbDY0Y2mNg4CyOBmEkgZg" alt="">
        </div>
        <h1>>> Salut 👋, moi c'est <span>Jessim</span> 
        <br> et je suis développeur! 
        <br> >> Bienvenue sur mon site!</h1>
    </div>
</template>
<script>
export default {
  name: 'InfoCard',
}
</script>
<style lang="css" scoped>
    .card{
        display:flex;
        flex-direction: row;
        align-items: center;
        flex-wrap: wrap;
        justify-content: space-evenly;
        padding: 10px;
        background-color: yellow;
        padding: 50px;
        border-bottom: 10px solid #2c3e50;
         cursor: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg'  width='40' height='48' viewport='0 0 100 100' style='fill:black;font-size:24px;'><text y='50%'>👋</text></svg>")
        16 0,
        auto;
    }
    h1{
        text-align: left;
        font-size: 3em;
    }
    h1 span {
        color: red;
    }
    .card__profile{
        display:flex;
        align-items: center;
    }
    .card__profileImage{
        max-width: 215px;
        /* border-radius: 60px; */
        /* border: 10px solid yellow; */
        box-shadow: 11px 11px 0px 0px #2c3e50;
    }
    .card__profileSocials{
        list-style: none;
        margin-left: -20px;
    }
    .card__profileSocials li{
        padding-top: 10px;
        padding-bottom: 10px;
    }
    .card__profileSocials li img{
        max-width: 40px;
    }
    .banner{
        display:flex;
        align-items: center;
        width: 100%;
    }
    .banner ul{
        padding: 0;
        width:100%;
        display:flex;
        list-style: none;
        flex-wrap: wrap;
        justify-content: space-evenly;
    }
    .banner ul li img{
        max-height: 40px;
        padding: 5px;
    }

</style>