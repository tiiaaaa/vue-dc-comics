<template>
    <div id="main-content">

        <MainContentJumbotron/>
        <MainContentCard/>

    </div>
</template>

<script>
import MainContentJumbotron from './MainContentJumbotron.vue';
import MainContentCard from './MainContentCard.vue';

export default {
    name: 'MainContent',
    components:{
        MainContentJumbotron,
        MainContentCard
    },
}
</script>

<style lang='scss' scoped>
    @import '../assets/scss/partials/_variables.scss';

    div#main-content{
        background-color: $darkColor;
    }
    
</style>