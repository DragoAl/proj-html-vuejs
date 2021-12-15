<template>
    <section>
        <div id="ourTreat">OUR TREATMENTS</div>
        <TreatmentCard
        v-for="treatment, i in treatmentsList " :key="i"
        :details='treatment'
        />
        <div id="backImg-cont">
            <div class="backImg-treat" id="backImgTop"></div>
            <div class="backImg-treat" id="backImgCenter">
                <p>“If you want to relax, watch the clouds pass by if you’re laying on the grass, or sit in front of the creek; just doing nothing and having those still moments is what really rejuvenates the body…”.</p>  
                <div> <strong>FRIEDA FRIEDSON</strong> , MASSEUSE</div> 
            </div>
            <div class="backImg-treat" id="backImgBottom"></div>
        </div>
        <div id="specialOffer">
            
            <div class="discount">25% <span>SPECIAL OFFER</span></div>
                <div class="mood">Take some time. Treat yourself. You deserve it.
                <span>Book a treatment this month and receive a 25% on all further treatments</span>
            </div>
            
           
            <button class="btn btn-bookNow">BOOK NOW</button>
        </div>
       

    </section>
</template>

<script>
import TreatmentCard from './TreatmentCard.vue'

export default {
    name: 'TreatmentsSection',
    components: {
        TreatmentCard
    },
    data () {
        return {
            treatmentsList: [
                {
                    img: 'Layer-1-new-400x440.jpg',
                    treatName: 'Hydrotherapy',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-2-new-400x440.jpg',
                    treatName: 'Massage',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-3-new-400x440.jpg',
                    treatName: 'Aromatherapy',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-4-new-400x440.jpg',
                    treatName: 'Heat Therapy',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-5-new-400x440.jpg',
                    treatName: 'Skin Care',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-6-new-400x440.jpg',
                    treatName: 'Spa Days',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'layer8-new-400x440.jpg',
                    treatName: 'Beauty Treatments',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
                
                {
                    img: 'Layer-7-new-400x440.jpg',
                    treatName: 'Residential',
                    treatScope: 'Vestibulum nec velit ante. Praesent dignissim interdum est, in lacinia elit pretium nec. Aliquam erat voluptat. Fusce laoreet mi leo.'
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
section {
    display: flex;
    flex-wrap: wrap;
   
}

#ourTreat {
    font-family: 'Libre Baskerville', serif;
    height: 150px;
    width: 100%;
    background-image:url("../assets/img/ptb_cta-new.jpg") ;
    line-height: 150px;
    vertical-align: middle;
    font-size: 28px;
    color: white;
}

#backImg-cont {
    width: 100%;
    height: 600px;
}

.backImg-treat {
    background-image: url("../assets/img/Home-quota-new.jpg");
}

#backImgTop {
    height: 150px;
    background-position: top;
   
}

#backImgCenter {
    height: 300px;
    background-position: center;
    color: white;
    font-style: italic;
    font-weight: bold;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 0 35%;
    
    div {
        margin: 20px 0;
    }
    
}

#backImgBottom {
    height: 150px;
    background-position: bottom;
}

#specialOffer {
    height: 300px;
    width: 100%;
    background-image:url("../assets/img/ptb_cta-new.jpg") ;
    background-size: cover;
    display: flex;
    justify-content: center;
    align-items: center;

    .discount {
        width: 120px;
        height: 100px;
        border: 1px solid white;
        font-size: 42px;
        color: white;
        padding: 10px;
        
        span {
            display: block;
            font-size: 10px;
            font-weight: bold;
        }
    }

    .mood {
        font-family: 'Libre Baskerville', serif;
        font-size: 28px;
        font-style: italic;
        color: white;
        text-align: left;
        margin: 0 20px;

        span {
            font-family: Avenir, Helvetica, Arial, sans-serif;
            font-style: normal;
            font-size: 16px;
            display: block;
            margin-top: 10px;
        }

    }

    .btn-bookNow {
        color: white;
        font-size: 12px;
        padding: 7px 20px;
        background-color: #b9afa1;
        margin-left: 100px;
        
        &:hover {
        background-color:#33a7b9;
  }

    }
    


}

</style>