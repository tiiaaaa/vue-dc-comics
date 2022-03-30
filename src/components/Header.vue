<template>
    <div class="header">
        <section class="my-container flex-header">
            <div id="logo-wrapper">
                <img src="../assets/img/dc-logo.png" alt="Logo Dc Comics">
            </div>

            <nav id="navbar-list">
                <ul>
                    <li v-for="(link, index) in headerLinks" :key="index"
                    :class="{'active' : link.active}">
                        <a href="#">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </section>
    </div>
</template>

<script>
export default {
    name: 'IndexHeader',
    data: function(){
        return{
            headerLinks:[
                {
                    text: "carachters",
                    url:"#",
                    active: false
                },

                {
                    text: "comics",
                    url:"#",
                    active: true
                },

                {
                    text: "movies",
                    url:"#",
                    active: false
                },

                {
                    text: "tv",
                    url:"#",
                    active: false
                },

                {
                    text: "games",
                    url:"#",
                    active: false
                },

                {
                    text: "collectibles",
                    url:"#",
                    active: false
                },

                {
                    text: "videos",
                    url:"#",
                    active: false
                },

                {
                    text: "fans",
                    url:"#",
                    active: false
                },

                {
                    text: "news",
                    url:"#",
                    active: false
                },

                {
                    text: "shop",
                    url:"#",
                    active: false
                },
            ]
        }
    }
}
</script>

<style lang='scss' scoped>
    @import '../assets/scss/partials/_variables.scss';

    div.header{
        height: 13vh;

        section.my-container{
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;
        }

        div#logo-wrapper{
            height: 80px;
            width: 80px;

            img{
                width: 100%;
            }
        }

        nav#navbar-list{
            height: 100%;
            ul{
                display: flex;
                height: 100%;

                li{
                    list-style-type: none;
                    margin-left: 1.2rem;
                    height: 100%;

                    &:active,
                    &.active{
                        border-bottom: 3px solid $primaryColor;
                    }

                    a{
                        font-size: 0.7rem;
                        font-weight: 600;
                        text-decoration: none;
                        text-transform: uppercase;
                        line-height: 90px;
                        color: black;
                    }
                }
            }
        }
    }
</style>