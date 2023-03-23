<script>
export default {
    data() {
        return {
            linkList: [
                {
                    name: "CHARACTERS",
                    link: "#",
                    target: "_self"
                },
                {
                    name: "COMICS",
                    link: "#",
                    target: "_self"
                },
                {
                    name: "MOVIES",
                    link: "#",
                    target: "_self"
                },
                {
                    name: "TV",
                    link: "#",
                    target: "_self"
                },
                {
                    name: "GAMES",
                    link: "#",
                    target: "_self"
                },
                {
                    name: "COLLECTIBLES",
                    link: "#",
                    target: "_self"
                },
                {
                    name: "VIDEOS",
                    link: "#",
                    target: "_self"
                },
                {
                    name: "FANS",
                    link: "#",
                    target: "_self"
                },
                {
                    name: "NEWS",
                    link: "#",
                    target: "_self"
                },
                {
                    name: "SHOP",
                    link: "#",
                    target: "_self"
                }
            ]
        }
    }
}
</script>

<template>
    <nav>
        <ul>
            <li v-for="element in linkList">
                <a :href="element.link" :target="element.target">{{ element.name }}</a>
            </li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
@use "../styles/colors.scss" as *;
@use "../styles/reset.scss" as *;


nav {
    height: 103px;

    ul {
        display: flex;
        align-items: center;
        list-style-type: none;
        height: 100%;

        li {
            display: flex;
            align-items: center;
            padding: 5px;
            margin: 5px;
            font-size: 0.925rem;
            height: 100%;
            position: relative;
            letter-spacing: -1px;

            &:last-child {
                margin-right: 0;
                padding-right: 0;
            }

            a {
                text-decoration: none;
                color: $secondary-color;
                font-weight: bold;

                &:hover {
                    color: $bg-alt-color;
                    transition: color .20s;
                }

                &::after {
                    content: "";
                    position: absolute;
                    width: 0;
                    left: 0;
                    background-color: $bg-alt-color;
                    height: 5px;
                    bottom: 0;
                    transition: ease .40s;
                }

                &:hover::after {
                    width: 100%;
                }
            }
        }
    }   
}

</style>