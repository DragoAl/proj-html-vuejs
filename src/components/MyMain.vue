<template>
<div id="jumbotron">
    <!-- <img src="@/assets/img/avada-spa-slider-image-1-new.jpg" alt=""> -->
    <div>
        <span>Give yourself permission</span>
        <h1>Relax, Revive e Rejuvenate</h1>
        <button class="btn btn-colored">EXPLORE TREATMENTS</button>
    </div>

</div>
    
</template>

<script>
export default {
    name:'MyMain'
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
        color: white;
    }
    h1{
        font-size: 55px;
        color: white;
    }
}
.btn {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    font-size: 14px;
    width: 200px;
    padding: 10px 15px;
    border-radius: 20px;
    border: none;
    margin: 10px 0;
}
.btn-colored {
    background-color:#d3cac0;
    color: white;
    font-weight: 1000;
}

</style>