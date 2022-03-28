<template>
    <div class="header">
        <div id="logo-wrapper">
            <img src="../assets/img/dc-logo.png" alt="Logo Dc Comics">
        </div>

        <nav id="navbar-list">
            <ul>
                <li v-for="(link, index) in headerLinks" :key="index">
                    <a href="#">{{ link.text }}</a>
                </li>
            </ul>
        </nav>

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
                    current: false
                },

                {
                    text: "comics",
                    url:"#",
                    current: true
                },

                {
                    text: "movies",
                    url:"#",
                    current: false
                },

                {
                    text: "tv",
                    url:"#",
                    current: false
                },

                {
                    text: "games",
                    url:"#",
                    current: false
                },

                {
                    text: "collectibles",
                    url:"#",
                    current: false
                },

                {
                    text: "videos",
                    url:"#",
                    current: false
                },

                {
                    text: "fans",
                    url:"#",
                    current: false
                },

                {
                    text: "news",
                    url:"#",
                    current: false
                },

                {
                    text: "shop",
                    url:"#",
                    current: false
                },
            ]
        }
    }
}
</script>

<style lang='scss' scoped>
    div.header{
        height: 15vh;
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: aqua;

        div#logo-wrapper{
            height: 80px;
            width: 80px;

            img{
                width: 100%;
            }
        }

        nav#navbar-list{
            ul{
                display: flex;

                li{
                    list-style-type: none;
                    margin-left: 1.2rem;

                    a{
                        font-size: 0.8rem;
                        text-decoration: none;
                        text-transform: uppercase;
                        color: black;
                    }
                }
            }
        }
    }
</style>