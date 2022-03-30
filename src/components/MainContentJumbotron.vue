<template>
    <div id="main-content-jumbotron">
        <img src="../assets/img/jumbotron.jpg" alt="Jumbotron immage">
    </div>
</template>

<script>
export default {
    name:'MainContentJumbotron',
}
</script>

<style lang='scss' scoped>

    div#main-content-jumbotron{
      height: 50vh;

      img{
        width: 100%;
        min-width: 1500px;
        height: 100%;
        object-fit: cover;
        object-position: top;
      }
    }

</style>