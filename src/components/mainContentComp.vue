<script>
import cardComp from './cardComp.vue';

export default {
    data() {
        return {
            cardList: [
                {
                    thumb: "https://static.dc.com/2023-03/LEGIONOB_Cv1_00111_DIGITAL.jpg?w=640",
                    price: "$19.99",
                    series: "DC'S LEGION OF BLOOM",
                    type: "comic book"
                },
                {
                    thumb: "https://static.dc.com/2023-03/FLS_Cv795_79511_DIGITAL.jpg?w=640",
                    price: "$3.99",
                    series: "THE FLASH",
                    type: "comic book"
                },
                {
                    thumb: "https://static.dc.com/2023-03/NTW_Cv102_10211_DIGITAL-1.jpg?w=640",
                    price: "$16.99",
                    series: "NIGHTWING",
                    type: "graphic novel"
                },
                {
                    thumb: "https://static.dc.com/2023-03/BMSMWF_Cv13_01311_DIGITAL.jpg?w=640",
                    price: "$2.99",
                    series: "BATMAN/SUPERMAN: WORLD'S FINEST",
                    type: "comic book"
                },
                {
                    thumb: "https://static.dc.com/2023-03/CTW_Cv53_05311_DIGITAL.jpg?w=640",
                    price: "$3.99",
                    series: "CATWOMAN",
                    type: "comic book"
                },
                {
                    thumb: "https://static.dc.com/2023-03/BA_Cv9_00911_DIGITAL.jpg?w=640",
                    price: "$2.99",
                    series: "BLACK ADAM",
                    type: "comic book"
                },
                {
                    thumb: "https://static.dc.com/2023-03/SM_LOST_Cv1_00111_DIGITAL.jpg?w=640",
                    price: "$3.99",
                    series: "SUPERMAN: LOST",
                    type: "comic book"
                },
                {
                    thumb: "https://static.dc.com/2023-03/SUPES_Cv2_00211_DIGITAL.jpg?w=640",
                    price: "$4.99",
                    series: "SUPERMAN",
                    type: "comic book"
                },
                {
                    thumb: "https://static.dc.com/2023-03/ROBIN_v3%20%28Cover%29.jpg?w=640",
                    price: "$5.99",
                    series: "ROBIN VOL. 3: SECRETS AND SHADOWS ",
                    type: "comic book"
                },
                {
                    thumb: "https://static.dc.com/2023-03/HQv3%20%28%20Cover%29.jpg?w=640",
                    price: "$6.99",
                    series: "HARLEY QUINN VOL. 3: VERDICT",
                    type: "comic book"
                },
                {
                    thumb: "https://static.dc.com/2023-03/MULTVTJ%20%28COVER%29.jpg?w=640",
                    price: "$4.99",
                    series: "MULTIVERSITY: TEEN JUSTICE",
                    type: "comic book"
                },
                {
                    thumb: "https://static.dc.com/2023-03/WW_Cv797_79711_DIGITAL.jpg?w=640",
                    price: "$16.99",
                    series: "WONDER WOMAN",
                    type: "graphic novel"
                }
            ]
        }
    },

    components: {
        cardComp,
    }
}
</script>

<template>
    <section class="main-content-ctn">
        <div class="top"></div>
        <div class="container">
            <div class="category">CURRENT SERIES</div>
            <cardComp v-for="card in cardList"  :image="card.thumb"
                :worth="card.price"
                :name="card.series"
                :genre="card.type" />
        </div>
        <div class="btn-ctn">
            <button>Load More</button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../assets/styles/colors.scss" as *;

.main-content-ctn {
    background-color: $secondary-color;
    
    .top {
        height: 50vh;
        background-image: url(../../public/img/jumbotron.jpg);
    }

    .category {
        font-weight: bolder;
        font-size: 1.4rem;
        letter-spacing: -1px;
        padding: 15px 30px;
        background-color: $bg-alt-color;
        max-width: 280px;
        position: absolute;
        top: -28px;
        left: -15px;
        z-index: 10px;
    }
    .container {
        position: relative;
        background-color: $secondary-color;
        max-width: 1300px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        padding: 40px 0;
    }

    .btn-ctn {
        text-align: center;
        padding: 20px;

        button {
            padding: 14px;
            width: 250px;
            border: 0;
            background-color: $bg-alt-color;
            font-weight: bold;
            font-size: 1rem;
            letter-spacing: -1px;
            color: $primary-color;

            &:hover {
                cursor: pointer;
                background-color: transparent;
                border: 2px solid $bg-alt-color;
                transition: background-color .40s;
            }
        }
    }
}

</style>