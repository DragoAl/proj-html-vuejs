<template>
    <div class="card" >
        <div class="img-box">        
            <img :src="require(`@/assets/img/${details.img}`)" :alt="details.treatName">
            <div class="backgroundHover"> {{details.treatName}}</div>
        </div>
        
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
    
    &:hover img{
        display: none;
    }
    
    &:hover .backgroundHover {
        display: block;
    }

    .backgroundHover {
        font-family: 'Libre Baskerville', serif;
        font-size: 36px;
        font-style: italic;
        color:white ;
        display: none;
        background-color:#b9afa1 ;
        width: 100%;
        height: 100%;
        text-align: center;
        vertical-align: middle;
        line-height: 500px ;
    }


    .img-box {
        height: 500px;
        

        img {
            width: 100%;
            height: 100%;
        }
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