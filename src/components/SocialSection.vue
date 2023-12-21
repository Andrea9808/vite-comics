<script>
export default {
    name: "SocialSection",

    data() {
        return {
            links: [
                {
                    img: "public/img/footer-facebook.png",
                    url: "#"
                },
                {
                    img: "public/img/footer-periscope.png",
                    url: "#"
                },
                {
                    img: "public/img/footer-pinterest.png",
                    url: "#"
                },
                {
                    img: "public/img/footer-twitter.png",
                    url: "#"
                },
                {
                    img: "public/img/footer-youtube.png",
                    url: "#"
                }
            ]
        }
    }
}
</script>

<template>
    <div class="bg">
        <div>
            <button>SIGN-UP NOW!</button>
        </div>

        <div>
            <ul>
                <h5><strong>FOLLOW US</strong></h5>
                <li v-for="link in links">
                    <a href="link.url">
                        <img :src="link.img" alt="">
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>




<style lang = 'scss' scoped>
@use '../Styles/partials/_variables.scss' as *;
@use '../Styles/partials/mixins' as *;

.bg {
    background-color: rgb(39 35 35);
    @include between;
    padding: 20px 210px;
}

h5 {
    color: blue;
    font-size: 15px;
    margin-right: 20px;
}

img {
    width: 30px;
    margin-right: 10px;
}

ul {
    display: flex;
    align-items: center;

    li {
        list-style-type: none;
    }
}

button {
    background-color: transparent;
    border: 1px solid blue;
    color: white;
    padding: 10px;
}
</style>
