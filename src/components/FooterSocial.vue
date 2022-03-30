<template>
    <div id="footer-social">
        <section class="my-container">
            
            <a href="#" class="btn">
                sign-up now!
            </a>
            
            <div class="flex-wrap">
                <a href="#" class="follow">
                    follow us
                </a>

                <a href="#" class="rounded-btn">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </a>

                <a href="#" class="rounded-btn">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </a>

                <a href="#" class="rounded-btn">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </a>

                <a href="#" class="rounded-btn">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </a>

                <a href="#" class="rounded-btn">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </a>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name:'FooterSocial'
}
</script>

<style lang='scss' scoped>
@import '../assets/scss/partials/_variables.scss';

    div#footer-social{
        padding: 1.5rem 0;
        background-color: $darkColor;

        section.my-container{
            display: flex;
            justify-content: space-between;

            a.btn{
                padding: .8rem;
                border: 3px solid $primaryColor;
                color: white;
                text-decoration: none;
                text-transform: uppercase;
                font-size: .8rem;
            }

            div.flex-wrap{
                display: flex;
                align-items: center ;
                justify-content: space-evenly;
                width: 35%;

                a.follow{
                    text-decoration: none;
                    text-transform: uppercase;
                    font-weight: 700;
                    color: $primaryColor;
                }

                a.rounded-btn{
                    display: inline-block;

                    img{
                    width: 30px;
                }
                }
            }
        }
    }
</style>