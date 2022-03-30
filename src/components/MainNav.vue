<template>
    <nav id="main-nav">
        <section class="my-container">
            <ul>
                <li v-for="(element, index) in listItem" :key="index">
                    <a :href="element.url">
                        <img :src="require(`@/assets/img/${element.immage}`)" alt="">
                        <span>{{element.text}}</span>
                    </a>
                </li>
            </ul>
        </section>
    </nav>
</template>

<script>
export default {
    name: 'MainNav',
        data: function(){
        return{
            listItem:[
                {
                    text: "digital comics",
                    url:"#",
                    immage: "buy-comics-digital-comics.png",
                    current: "",
                },

                {
                    text: "dc merchandise",
                    url:"#",
                    immage: "buy-comics-merchandise.png",
                    current: "",
                },

                {
                    text: "subscription",
                    url:"#",
                    immage: "buy-comics-shop-locator.png",
                    current: "",
                },

                {
                    text: "comic shop locator",
                    url:"#",
                    immage: "buy-comics-subscriptions.png",
                    current: "",
                },

                {
                    text: "dc power visa",
                    immage: "buy-dc-power-visa.svg",
                    current: "",
                },
            ]
        }
    }
}
</script>

<style  lang='scss' scoped>
    @import '../assets/scss/partials/_variables.scss';

    nav#main-nav{
        height: 16vh;
        background-color: $primaryColor;

        section.my-container{
            height: 100%;
        }

        ul{
            display: flex;
            justify-content: space-around;
            height: 100%;

            li{
                list-style-type: none;
                display: flex;
                align-items: center;
                padding: .8rem;
                
                a{
                    display: flex;
                    text-decoration: none;
                    color: white;
                    
                    img{
                        height: 50px;
                        margin-right: 1rem;
                    }
                    
                    span{
                        text-transform: uppercase;
                        line-height: 45px;
                        font-size: 0.7rem;
                        font-weight: 600;
                    }
                }
            }
        }
    }

</style>