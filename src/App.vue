<script>
import headerComp from './components/headerComp.vue';
import mainComp from './components/mainComp.vue';
import footerComp from './components/footerComp.vue';

export default {
    components: {
        headerComp,
        mainComp,
        footerComp
    }
}

</script>

<template>
    <headerComp></headerComp>
    <mainComp></mainComp>
    <footerComp></footerComp>
</template>

<style lang="scss">
@use "./styles/colors.scss" as *;
@use "./styles/reset.scss" as *;

</style>
