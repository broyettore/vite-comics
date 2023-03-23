<script>
export default {
    data() {
        return {
            btnText: "SIGN-UP NOW!",
            ctaText: "FOLLOW US",
            link: "#",
            socialList: [
                "../../public/img/footer-facebook.png",
                "../../public/img/footer-twitter.png",
                "../../public/img/footer-youtube.png",
                "../../public/img//footer-pinterest.png",
                "../../public/img/footer-periscope.png",
            ]
        }
    },
}
</script>

<template>
    <section class="footer-bottom">
        <div class="container">
            <div class="left">
                <button>{{ btnText }}</button>
            </div>
            <div class="right">
                <div class="cta">
                    <span>
                        <a :href="link">
                            {{ ctaText }}
                        </a>
                    </span>
                </div>
                <div class="socials">
                    <div class="icon-ctn" v-for="element in socialList">
                        <a :href="link">
                            <img :src="element" :alt="link">
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/colors.scss" as *;
@use "../styles/reset.scss" as *;

.footer-bottom {
    background-color: $footer-bg-color;
    padding: 40px;
    color: $primary-color;

    .container {
        max-width: 1300px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        a {
            text-decoration: none;

            &:hover {
                cursor: pointer;
            }
        }

        .left {
            button {
                background-color: transparent;
                border: 2px solid $bg-alt-color;
                padding: 12px 24px;
                color: $primary-color;
                font-size: 1rem;
                font-weight: bold;
                
                &:hover {
                    cursor: pointer;
                    transform: translateY(-6px);
                    transition: ease .40s;
                }
            }
        }

        .right {
            display: flex;
            justify-content: flex-end;
            align-items: center;
            width: 60%;
            
            .cta {
                font-size: 1.2rem;
                font-weight: bold;
                color: $bg-alt-color;
                letter-spacing: -1px;
                padding: 10px;
                margin-right: 15px;
            }

            .socials {
                display: flex;
                justify-content: space-between;
                width: 30%;
            }
        }
    }
}

</style>