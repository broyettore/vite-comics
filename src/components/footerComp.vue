<script>
import footerTop from './footerTop.vue';
import footerBottom from './footerBottom.vue';

export default {
    components: {
        footerTop,
        footerBottom
    }
}
</script>

<template>
    <footerTop></footerTop>
    <footerBottom></footerBottom>
</template>

<style lang="scss" scoped>
@use "../assets/styles/colors.scss" as *;
</style>