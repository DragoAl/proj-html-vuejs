<template>
    <footer>
        <img src="../assets/img/avada-spa-logo-retina-new-400x46.png" alt="logo">
        <div class="info">
            <span class="info-setting" v-for="info, i in infoFooter" :key="i"> <i :class="info.infoIcon"></i> {{info.infoName}}</span>
        </div>
        <div class="social">
            <div class="socialLogo-container" v-for="social, i in socialLogos" :key="i">
                <a :href="social.url"><i :class="social.socialIcon"></i></a>
            </div>
        </div>

        <div id="toTopOfPage">
            <a href="#"><i class="fas fa-chevron-up"></i></a>
        </div>

     </footer>
</template>

<script>
export default {
    name: 'MyFooter',
    props: {
        socialLogos:Array,
        infoFooter:Array
    }
}
</script>

<style scoped lang="scss">
footer {
    position: relative;
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 100px;
    border-top: 8px solid #c2c2c6;

    img {    
        height: 30%;
    }

    .info {
        width: 40%;
    
        .info-setting {
            text-transform: uppercase;
            font-size: 12px;
            color: #b7bac4;

            &::after {
                content: ' |';
            }
        }   
    }
    
    .social {
        display: flex;
        
        .socialLogo-container {
            background-color:#e8e8e8 ;
            border-radius: 20%;
            margin: 0 5px;
            width: 40px;
            height: 40px;
            line-height: 40px;
            vertical-align: middle;
            cursor: pointer;

            a {
                color: #bfbfbf;
                text-decoration: none;
            }
        }
    }

    #toTopOfPage {
        position: absolute;
        bottom: 0px;
        right: 7%;
        width: 30px;
        height: 18px;
        background-color: #474747;
        border-radius: 3px 3px 0 0;

        a {
            text-decoration: none;
            color: white;
        }
    }
}

</style>