<template>
    <div id="footer-contact">
        <section class="my-container">
            <div id="wrap-list">
                <ul>
                    <li class="title-argument">dc comics
                        <ul class="nasted-ul">
                            <li><a href="#">characters</a></li>
                            <li><a href="#">movies</a></li>
                            <li><a href="#">characters</a></li>
                            <li><a href="#">tv</a></li>
                            <li><a href="#">games</a></li>
                            <li><a href="#">videos</a></li>
                            <li><a href="#">news</a></li>
                        </ul>
                    </li>

                    <li class="title-argument">shop
                        <ul class="nasted-ul">
                            <li><a href="#">shop dc</a></li>
                            <li><a href="#">shop dc collectibles</a></li>
                        </ul>
                    </li>
                </ul>

                <ul>
                    <li class="title-argument">dc
                        <ul class="nasted-ul">
                            <li><a href="#">term of use</a></li>
                            <li><a href="#">privacy policy (new)</a></li>
                            <li><a href="#">ad choices</a></li>
                            <li><a href="#">advertising</a></li>
                            <li><a href="#">jobs</a></li>
                            <li><a href="#">subscriptions</a></li>
                            <li><a href="#">talent workshops</a></li>
                            <li><a href="#">cpsp certificates</a></li>
                            <li><a href="#">ratings</a></li>
                            <li><a href="#">shop help</a></li>
                            <li><a href="#">contact us</a></li>
                        </ul>
                    </li>
                </ul>

                <ul>
                    <li class="title-argument">sites
                        <ul class="nasted-ul">
                            <li><a href="#">dc</a></li>
                            <li><a href="#">mad magazine</a></li>
                            <li><a href="#">dc kids</a></li>
                            <li><a href="#">dc universe</a></li>
                            <li><a href="#">dc power visa</a></li>
                        </ul>
                    </li>
                </ul>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name:'FooterContact'
}
</script>

<style lang='scss' scoped>
    
    div#footer-contact{
        padding: 1.5rem 0;
        background-image: url("../assets/img/footer-bg.jpg");

        div#wrap-list{
            display: flex;

            ul{
            padding: 1rem;

            li.title-argument{
                list-style-type: none;
                text-transform: uppercase;
                margin-bottom: 1rem;
                font-size: .9rem;
                font-weight: 600;
                color: white;

                ul.nasted-ul{
                    margin-top: .8rem;
                    padding: 0;

                    li{
                        list-style-type: none;

                        a{
                            font-size: .6rem;
                            font-weight: 100;
                            text-decoration: none;
                            text-transform: capitalize;
                            color: rgb(189, 181, 181);
                        }
                    }
                }
            }
        }
        }
    }

</style>