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

</style>