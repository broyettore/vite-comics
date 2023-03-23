<script>
export default {
    data() {
        return {
            optionsList: [
                {
                    icon: "../",
                    title: "DIGITAL COMICS"
                },
                {
                    icon: "#",
                    title: "DC MERCHANDISE"
                },
                {
                    icon: "#",
                    title: "SUBSCRIPTION"
                },
                {
                    icon: "#",
                    title: "COMIC SHOP LOCATOR"
                },
                {
                    icon: "#",
                    title: "DC POWER VISA"
                }
            ] 
        }
    }
}
</script>

<template>
    <section class="options-ctn">
        <div class="container">

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/colors.scss" as *;
@use "../styles/reset.scss" as *;

.options-ctn {
    background-color: $bg-alt-color;
}

.container {
    max-width: 1300px;
    margin: 0 auto;
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>