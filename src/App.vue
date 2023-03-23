<script>
import header from './components/header.vue';
import main from './components/main.vue';
import options from './components/options.vue';
import footer from './components/footer.vue';

export default {
    components: {
        header,
        main,
        options,
        footer
    }
}

</script>

<template>
    <header></header>
    <main></main>
    <options></options>
    <footer></footer>
</template>

<style lang="scss" scoped>
@use "./styles/general.scss" as *;

</style>
