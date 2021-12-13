<template>
<nav>
    <i class="fas fa-home"></i>
    <div v-for= "element, i in menuElements.slice(0,2) " :key='i'>
        <i :class="element.icon"></i>
        <h5>{{element.title}}</h5>
        <span>{{element.subtitle}}</span>
    </div>
    <img src="../assets/img/avada-spa-logo-retina-new-400x46.png" alt="">
    <div v-for= "element, i in menuElements.slice(2,4) " :key='i'>
        <i :class="element.icon"></i>
        <h5>{{element.title}}</h5>
        <span>{{element.subtitle}}</span>
    </div>
    <i class="fas fa-plus"></i>

</nav>
    
</template>

<script>
export default {
    name: 'MyHeader',
    props : {
        menuElements: Array
    }

}
</script>

<style scoped lang="scss">

nav {
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    div {
        margin:0 25px;
        cursor: pointer;
    }
    i {
        color: #d3cac0;
    }
    img {
        height: 25px;
    }
    h5 {
        margin: 3px 0;
        color: #6b6a69;
    }
    span{
        font-size: 12px;
        color: #6c6c6c;
    }
}
.fa-home, .fa-plus {
    margin: 0 40px;
    color: #6b6a69;
}


</style>