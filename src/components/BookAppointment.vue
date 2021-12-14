<template>
    <section>
        <img src="@/assets/img/face_and_body_treatments-new-400x581.jpg" alt="face_and_body_treatments">
        <div id="sectionToBook">
            <h2>Face &amp; Body Treatments</h2>
            <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Alias unde id, dolorum  amet iure commodi nobis quo ipsam ea dolores quod doloremque corrupti?</p>
           
            <div class="price-service" id="massage">
                <div class="plus square" :class="{dispNone: NotActiveMassage}" @click.prevent="isActiveMassage"> +</div>
                <div class="minus square" :class=" {dispNone: activeMassage}" @click.prevent="isActiveMassage"> -</div>
                <span class="treatment-name">Oil Massage</span>
                <p class="treatments-info " :class=" {dispNone: activeMassage}"> <strong>$62 For 2 Hours </strong> - Lorem ipsum dolor sit amet</p>
            </div>

            <div class="price-service" id="manicure">
                <div class="plus square" :class="{dispNone: NotActiveMani}" @click.prevent="isActiveMani"> +</div>
                <div class="minus square " :class=" {dispNone: activeMani}" @click.prevent="isActiveMani"> -</div>
                <span class="treatment-name">Manicure</span>
                <p class="treatments-info " :class=" {dispNone: activeMani}"> <strong>$40 For 1 Hour</strong>  - Lorem ipsum</p>
            </div>

            <div class="price-service" id="aromatherapy">
                <div class="plus square" :class="{dispNone: NotActiveAroma}" @click.prevent="isActiveAroma"> +</div>
                <div class="minus square" :class=" {dispNone: activeAroma}" @click.prevent="isActiveAroma"> -</div>
                <span class="treatment-name">Aromatherapy</span>
                <p class="treatments-info " :class=" {dispNone: activeAroma}"><strong>$35 For 1/2 Hour</strong> - Lorem ipsum dolor sit</p>
            </div>

            <button id="bookApp" class="btn btn-empty">BOOK AN APPOINTMENT</button>
        </div>
    </section>
</template>
<script>
export default {
    name:'BookAppointment',
    data() {
        return {
            activeMassage: true,
            NotActiveMassage: false,
            activeMani: true,
            NotActiveMani: false,
            activeAroma: true,
            NotActiveAroma: false
        }
    },

    methods: {
        isActiveMassage() {
            this.activeMassage = !this.activeMassage
            this.NotActiveMassage = !this.NotActiveMassage
        },
        isActiveMani() {
            this.activeMani = !this.activeMani
            this.NotActiveMani = !this.NotActiveMani
        },

        isActiveAroma() {
            this.activeAroma = !this.activeAroma
            this.NotActiveAroma = !this.NotActiveAroma
        }
    }
}
</script>

<style scoped lang="scss">
section {
    text-align: left;
    background-color: #f9f9f9;
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 100px ;
    height: 800px;
    

    img {
        border: 20px solid white;
        box-shadow: 5px 5px 10px 0px #6c6c6c;
        width: 350px;
    }
    #sectionToBook {
        margin: 0 40px;
        width: 20%;
        h2 {
            font-family: 'Libre Baskerville', serif;
            font-size: 32px;
            font-weight: 200;
            color: #6c6c6c;



        }

        p{
            margin: 20px 0 40px;
            font-size: 14px;
        }

        .price-service {
            width: 300px;
            margin: 8px 0;
            min-height: 40px;
            padding: 10px;
            background-color: white;
            border: 1px solid lightgray;
        }

        .square {
            width: 16px;
            font-size: 12px;
            font-weight: bold;
            text-align: center;
            display: inline-block;
        }

        .plus {
            background-color: #6c6c6c;
            color: white;
        }

        .minus {
            background-color:#bcafa1;
            color: white;
        }

        .treatment-name {
            font-family: 'Libre Baskerville', serif;
            font-size: 14px;
            margin-left: 10px;
            font-style: italic;
            color: #bcafa1;
        }

        .treatments-info {
            font-size: 12px;
            margin: 10px 0;
        }

        .dispNone {
            display: none;
        }

        #bookApp {
            margin: 30px 0;
            font-size: 12px;
        }
    }
}

</style>