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
@use "../styles/colors.scss" as *;
@use "../styles/reset.scss" as *;
</style>