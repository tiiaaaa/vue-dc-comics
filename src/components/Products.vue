<template>
    <div>
        <div id="content"></div>
        <div id="gadjet-bar">
            <ul>
                <li v-for="(link, index) in gadjetLinks" :key="index">
                    <a href="#">
                        <div class="gadjet-img">
                            <img :src="link.immage" alt="">
                        </div>
                        <span>{{link.text}}</span>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'IndexProducts',
        data: function(){
        return{
            gadjetLinks:[
                {
                    text: "digital comics",
                    url:"#",
                    immage: "../assets/img/buy-comics-digital-comics.png",
                    current: "",
                },

                {
                    text: "dc merchandise",
                    url:"#",
                    current: "",
                },

                {
                    text: "subscription",
                    url:"#",
                    current: "",
                },

                {
                    text: "comic shop locator",
                    url:"#",
                    current: "",
                },

                {
                    text: "dc power visa",
                    url:"#",
                    current: "",
                },
            ]
        }
    }
}
</script>

<style  lang='scss' scoped>
    div#content{
        height: 13vh;
        background-color: black;
    }

    div#gadjet-bar{
        height: 15vh;
        display: flex;
        align-items: center;
        background-color: rgb(48, 82, 231);

        ul{
            display: flex;
            li{
                list-style-type: none;
                a{
                    display: flex;
                    text-decoration: none;
                    color: white;
                    div.gadjet-img{
                        width: 35px;
                        margin-right: 1rem;
                        img{
                            width: 100%;
                        }
                    }

                    span{
                        text-transform: uppercase;
                        font-size: 0.7rem;
                    }
                }
            }
        }
    }

</style>