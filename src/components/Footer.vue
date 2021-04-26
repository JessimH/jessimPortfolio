<template>
    <div class="footer">
        <h4>made with ♥️ ( and a lot of redbull  )</h4>
         <div>
                <ul class="card__profileSocials">
                    <li><a target="_blank" href="https://github.com/JessimH"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/91/Octicons-mark-github.svg/1024px-Octicons-mark-github.svg.png" alt=""></a></li>
                    <li><a target="_blank" href="https://www.linkedin.com/in/jessim-heddadi-962734177/"><img src="https://www.exakis-nelite.com/wp-content/uploads/sites/12/2018/11/logo-LinkedIn.png" alt=""></a></li>
                    <li><a target="_blank" href="https://www.instagram.com/jessimheddadi/"><img src="http://assets.stickpng.com/images/580b57fcd9996e24bc43c521.png" alt=""></a></li>
                </ul>
            </div>
    </div>
</template>
<script>
export default {
  name: 'Footer',
    
}
</script>
<style lang="css" scoped>
    .footer {
        border-top: 10px solid #2c3e50;
        background-color:yellow;
        height: fit-content;
        display:flex;
        flex-direction: column;
        align-items:center;
        justify-content:center;
        width:100vw;
    }
    .card__profileSocials{
        display:flex;
        list-style: none;
        margin-left: -20px;
    }
    .card__profileSocials li{
        padding-top: 10px;
        padding-bottom: 10px;
        margin-left: 10px;
    }
    .card__profileSocials li img{
        max-width: 40px;
        cursor: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg'  width='40' height='48' viewport='0 0 100 100' style='fill:black;font-size:24px;'><text y='50%'>📞</text></svg>")
            16 0,
            auto;
    }
</style>