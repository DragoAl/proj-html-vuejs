<template>
<section>
    <div id="jumbotron">
    <!-- <img src="@/assets/img/avada-spa-slider-image-1-new.jpg" alt=""> -->
    <div>
        <span>Give yourself permission</span>
        <h1>Relax, Revive e Rejuvenate</h1>
        <button class="btn btn-colored">EXPLORE TREATMENTS</button>
    </div>
</div>
    <OurApproach
    :typeOfServices= 'services'
    />
</section>

    
</template>

<script>
import OurApproach from '../components/OurApproach.vue'

export default {
    name:'MyMain',
    components: {
        OurApproach
    },
    data() {
        return {
            services: [
                {
                    icon: 'fas fa-sign-language',
                    serviceTitle:'Massages',
                    id: 1
                },
                {
                    icon: 'far fa-smile',
                    serviceTitle:'Therapy',
                    id: 2
                },
                {
                    icon: 'fas fa-heart',
                    serviceTitle:'Relaxing',
                    id: 3
                },
                {
                    icon: 'far fa-moon',
                    serviceTitle:'Meditation',
                    id: 4
                },
                {
                    icon: 'far fa-snowflake',
                    serviceTitle:'Natural Beauty',
                    id: 5
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
#jumbotron {
    font-family: 'Libre Baskerville', serif;

    height: 600px;
    background-size: 100% 600px;
    background-image: url("../assets/img/avada-spa-slider-image-1-new.jpg");
    display: flex;
    justify-content: center;
    align-items: center;
    // img {
    //     max-width: 100%;
    // }
    span {
        font-style: italic;
        font-size: 35px;
        color: #e9ddce;
    }
    h1{
        font-size: 55px;
        color: white;
    }
}


</style>