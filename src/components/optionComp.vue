<script>
export default {
    data() {
        return {
            optionsList: [
                {
                    icon: ".../../public/img/buy-comics-digital-comics.png",
                    title: "DIGITAL COMICS",
                    description: "dc icon"
                },
                {
                    icon: "../../public/img/buy-comics-merchandise.png",
                    title: "DC MERCHANDISE",
                    description: "t-shirt icon"
                },
                {
                    icon: "../../public/img/buy-comics-subscriptions.png",
                    title: "SUBSCRIPTION",
                    description: "thunder card"
                },
                {
                    icon: "../../public/img/buy-comics-shop-locator.png",
                    title: "COMIC SHOP LOCATOR",
                    description: "pointer icon"
                },
                {
                    icon: "../../public/img/buy-dc-power-visa.svg",
                    title: "DC POWER VISA",
                    description: "credit card icon"
                }
            ] 
        }
    }
}
</script>

<template>
    <section class="options-ctn">
        <div class="container">
            <div class="item" v-for="element in optionsList">
                <div class="img-ctn">
                    <img :src="element.icon" :alt="element.description">
                </div>
                <div class="title-ctn">
                    <h3>{{ element.title }}</h3>
                </div>
        </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/colors.scss" as *;
@use "../styles/reset.scss" as *;

.options-ctn {
    background-color: $bg-alt-color;

    .container {
        max-width: 1300px;
        margin: 0 auto;
        padding: 100px 0;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .item {
            width: 20%;
            display: flex;
            align-items: center;

            .title-ctn {
                width: 100%;
                font-size: 0.9rem;
            }

            .img-ctn {
                width: 30%;
                margin: 0 10px;

                img {
                    width: 95%;

                }
            }
        }
    }
}

</style>