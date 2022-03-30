<template>
    <div id="footer-social">
        <section class="my-container">
            
            <a href="#" class="btn">
                sign-up now!
            </a>
            
            <div>
                <a href=""></a>
                <a href=""></a>
                <a href=""></a>
                <a href=""></a>
                <a href=""></a>
                <a href=""></a>
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
        }
    }
</style>