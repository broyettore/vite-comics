<script>
export default {
    data() {
        return {
            link: "#",
            target: "_self",
            firstSectionList: 
                {
                    title: "DC COMICS",
                    list: [
                        "Characters",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Videos",
                        "News",
                    ]
                },
            secondSectionList: 
                {
                    title: "SHOP",
                    list: [
                        "Shop DC",
                        "Shp DC Collectibles",
                    ]
                },
            thirdSectionList: 
                {
                    title: "DC",
                    list: [
                        "Terms Of Use",
                        "Privacy policy (New)",
                        "Ad Choices",
                        "Advertising",
                        "Jobs",
                        "Subscriptions",
                        "Talent Workshops",
                        "CPSC Certificates",
                        "Ratings",
                        "Shop Help",
                        "Contact Us",
                    ]
                },
            fourthSectionList: 
                {
                    title: "SITES",
                    list: [
                        "DC",
                        "MAD Magazine",
                        "DC Kids",
                        "DC Universe",
                        "DC Power Visa",
                    ]
                }
            
        }
    }
}
</script>

<template>
    <section class="footer-top">
        <div class="container">
            <div class="left">
                <div class="top">
                    <h3>{{ firstSectionList.title }}</h3>
                    <ul>
                        <li v-for="element in firstSectionList.list">
                            <a :href="link" :target="target">{{ element }}</a>
                        </li>
                    </ul>
                </div>
                <div class="bottom">
                    <h3>{{ secondSectionList.title }}</h3>
                    <ul>
                        <li v-for="element in secondSectionList.list">
                            <a :href="link" :target="target">{{ element }}</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="center">
                <h3>{{ thirdSectionList.title }}</h3>
                <ul>
                    <li v-for="element in thirdSectionList.list">
                        <a :href="link" :target="target">{{ element }}</a>
                    </li>
                </ul>
            </div>
            <div class="right">
                <h3>{{ fourthSectionList.title }}</h3>
                <ul>
                    <li v-for="element in fourthSectionList.list">
                        <a :href="link" :target="target">{{ element }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use "../styles/colors.scss" as *;

.footer-top {
    background-image: url(../../public/img/dc-logo-bg.png), url(../../public/img/footer-bg.jpg);
    background-position: 75% 50%, bottom left;
    background-size: 35%, 100%;
    padding: 80px 0;
    background-repeat: no-repeat;
    color: $primary-color;

    .container {
        max-width: 1300px;
        margin: 0 auto;
        display: flex;
        justify-content: flex-start;
        align-items: flex-start;
        height: 100%;

            .left {
                .top {
                    margin-bottom: 25px;
                }
            }
            .left, .center {
                margin-right: 2rem;
            }

            h3 {
                margin-bottom: 20px;
            }

            ul {
                list-style-type: none;

                li {
                    margin: 8px 0;
                }
            }

            a {
                text-decoration: none;
                color: $text-alt-color;

                &:hover {
                    color: $bg-alt-color;
                    transition: color .30s;
                }
            }

}
}
</style>