<script>
import dcLogo from './dcLogo.vue';
import navBar from './navBar.vue';

export default {
    data() {
        return {
            // a 
        }
    },

    components: {
        dcLogo,
        navBar
    }
}
</script>

<template>
    <dcLogo></dcLogo>
    <navBar></navBar>
</template>

<style lang="scss" scoped>
@use "./styles/general.scss" as *;

</style>
