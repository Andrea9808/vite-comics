<script>
export default {
    name: "HeaderSection",

    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false
                },
                {
                    text: "TV",
                    url: "#",
                    current: false
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false
                }, {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false
                }
            ]
        }
    }
}
</script>

<template>
    <div class="bg">

        <div class="container">
            <div>
                <img class="logo" src="/public/img/dc-logo.png" alt="logoDC">
            </div>

            <div>
                <ul class="navbar">
                    <li v-for="link in links">
                        <a :href="link.url" :class="link.current ? 'active' : ''">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </div>
        </div>


    </div>
</template>




<style lang = 'scss' scoped>
@use '../Styles/partials/_variables.scss' as *;
@use '../Styles/partials/mixins' as *;

.bg {
    background-color: $primary;
    margin-top: 40px;
    
}

.container{
    @include around;
}

.logo {
    background-color: transparent;
    height: 50px;
    margin: 10px;
}

.navbar li {
    text-decoration: none;
    list-style-type: none;
    display: inline-block;

    a {
        text-decoration: none;
        margin-right: 10px;
        color: black;
    }
}

.active {
    color: blue;
    padding-bottom: 28px;
    border-bottom: 3px solid blue;
}
</style>
