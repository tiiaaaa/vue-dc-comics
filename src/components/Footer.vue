<template>
    <footer>
        footer

        <FooterContact/>
        <FooterSocial/>
    </footer>
</template>

<script>
import FooterContact from './FooterContact.vue';
import FooterSocial from './FooterSocial.vue';

export default {
    name: 'IndexFooter',
    components:{
        FooterContact,
        FooterSocial
    }
}
</script>

<style>

</style>