<script>
export default {
    props: {
        image: String,
        worth: String,
        name: String,
        genre: String
    }
}
</script>

<template>
            <div class="card-item">
                <div class="card-top">
                    <img :src="image" :alt="genre">
                </div>
                <div class="card-info">
                    <h4>{{ name }}</h4>
                    <h5>{{ worth }}</h5>
                </div>
            </div>
</template>

<style lang="scss" scoped>
@use "../assets/styles/colors.scss" as *;
.card-item {
    width: 16%;
    padding: 10px;

    &:hover {
            cursor: pointer;
            transform: scale(1.1);
            transition: ease .40s;
        }

    .card-top {
        height: 260px;
        width: 100%;

        img {
            width: 100%;
            height: 100%;
        }
    }

    .card-info {
        h4 {
            font-size: 0.975rem;
            letter-spacing: -1px;
        }

        h4, h5 {
            margin: 8px 0;
        }
    }
}
</style>