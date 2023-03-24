<script>
import dcLogo from './dcLogo.vue';
import navBar from './navBar.vue';

export default {
    components: {
        dcLogo,
        navBar
    }
}
</script>

<template>
    <header>
        <div class="container">
            <dcLogo></dcLogo>
            <navBar></navBar>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use "../assets/styles/colors.scss" as *;

.container {
    max-width: 1300px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

</style>
