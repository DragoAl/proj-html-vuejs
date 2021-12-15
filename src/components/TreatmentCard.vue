<template>
    <div class="card" >
        <img :src="require(`@/assets/img/${details.img}`)" :alt="details.treatName">
        <h3>{{details.treatName}}</h3>
        <div class="separator"></div>
        <p>{{details.treatScope}}</p>
    </div>
</template>

<script>
export default {
    name:'TreatmentCard',
    props : {
        details:Object
    }
}
</script>

<style scoped lang="scss">
.card{
    width:25%;
    text-align: left;
    border: 0.1em solid #dadada;
    cursor: pointer;

    img {
        width: 100%;
    }

    h3 {
        font-family: 'Libre Baskerville', serif;
        font-weight: 100;
        padding: 23px;
        color:#bcafa1 ;

    }
    p{
        padding: 23px;
    }
    .separator{
        width: 90%;
        margin: 0 auto;
        border: 0.1em dotted 	#dadada ;
        
    }
}

</style>