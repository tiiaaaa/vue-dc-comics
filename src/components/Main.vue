<template>
    <main>
        
        <MainContent/>
        <MainNav/>
    </main>
</template>

<script>
import MainNav from './MainNav.vue';
import MainContent from './MainContent.vue';
export default {
    name: 'IndexMain',
    components: {
        MainContent,
        MainNav
    }
}
</script>

<style lang='scss' scoped>

</style>