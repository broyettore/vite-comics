<script>
export default {
    data() {
        return {
            // a 
        }
    }
}
</script>

<template>
    <section class="footer-top">
        <div class="container"></div>
    </section>
    
</template>

<style lang="scss" scoped>
@use "../styles/colors.scss" as *;
@use "../styles/reset.scss" as *;

.footer-top {
    background: url(../../public/img/dc-logo-bg.png);
}

.container {
        max-width: 1300px;
        margin: 0 auto;
        display: flex;
}
</style>