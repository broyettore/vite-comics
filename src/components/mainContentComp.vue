<script>
export default {
    data() {
        return {
            content: "--> Content goes here <--"
        }
    }
}
</script>

<template>
    <section class="main-content-ctn">
        <div class="container">
            <h1> {{ content }}</h1>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/colors.scss" as *;

.main-content-ctn {
    background-color: $secondary-color;
    height: calc(100vh - 103px);

    .container {
        max-width: 1300px;
        margin: 0 auto;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
}

</style>