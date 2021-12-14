<template>
<section>
    <h2>Luxury Spa Experiences</h2>
    <div>
        <i class="fab fa-envira"></i>
        <p class="mission">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad rem, et nostrum hic commodi porro ex facere accusamus inventore autem doloremqu</p>
        <div id="separator"></div>
    </div>
    
    <div>
        <p class="info">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Perferendis in, ratione fuga illo est eveniet harum,  sequi? Amet necessitatibus dolorem pariatur neque.Lorem ipsum, dolor sit amet consectetur adipisicing elit. Perferendis in, ratione fuga illo est eveniet harum, cumque</p>
        <button class="btn btn-empty">OUR APPROACH</button>
    </div>

    
    <section id="services" >
        <div v-for="service, i in typeOfServices " :key='i' :class="service.id % 2 == 0 ? 'low' : ''">
            <i class="service-icon" :class="service.icon"></i>
            <span class="service-name">{{service.serviceTitle}}</span>
            
        </div>
        

    </section>
</section>
    
</template>

<script>
export default {
name : 'OurApproach',
props: {
    typeOfServices: Array
}
}
</script>

<style scoped lang="scss">
section{
    font-family: 'Libre Baskerville', serif;
    width: 60%;
    margin: 70px auto;
    
    h2 {
        font-size: 42px;
        font-weight: 400;
        color: #6c6c6c;
    }
    div {
        width: 90%;
        margin: 0 auto;
        
       
    }
    .mission {
        font-size: 14px;
        color:#bcafa1;
        font-style: italic;
        line-height: 20px;
    }

    .info {
        font-size: 10px;
        line-height: 20px;
    }

    i {
        margin: 20px 0;
        transform: scaleX(-1);
        font-size: 22px;
        color:#bcafa1
    }
    
    #separator {
        height: 2px;
        width: 50px;
        background-color: #bcafa1;
        margin: 30px auto;
    }

    p {
        padding: 0 250px;
        font-size: 12px;
    } 
    #services {
        display: flex;
        justify-content: center;
        div {
            cursor: pointer;
            margin:0px 40px;
            
            .service-icon {
                font-size: 28px;
            }
            
            .service-name {
                display:block;
                font-size: 12px;
                color: #6c6c6c;
                font-style:normal;
            }
        }

    }
    .low {
        padding: 40px 0;
    }
}


</style>