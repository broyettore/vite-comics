<script>
import mainContentComp from './mainContentComp.vue';
import optionComp from './optionComp.vue';

export default {
    data() {
        return {
            content: "--> Content goes here <--"
        }
    },

    components: {
        mainContentComp,
        optionComp
    }
}
</script>

<template>
    <main>
        <mainContentComp></mainContentComp>
        <optionComp></optionComp>
    </main>
</template>

<style lang="scss" scoped>
@use "../styles/colors.scss" as *;

main {
    color: $primary-color;
}
</style>