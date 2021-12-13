<template>
<nav>
    <i class="fas fa-home"></i>
    <div v-for= "element, i in menuElements " :key='i'>
        <i :class="element.icon"></i>
        <div>{{element.title}}</div>
        <div>{{element.subtitle}}</div>

    </div>
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
}


</style>