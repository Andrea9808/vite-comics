<script>

export default {
    name: "ShopSection",

    data() {
        return {
            links: [
                {
                    img: "public/img/buy-comics-digital-comics.png",
                    text: "DIGITAL COMICS",
                    url: "#"
                },
                {
                    img: "public/img/buy-comics-merchandise.png",
                    text: "DC MERCHANDISE",
                    url: "#"
                },
                {
                    img: "public/img/buy-comics-subscriptions.png",
                    text: "SUBSCRIPTION",
                    url: "#"
                },
                {
                    img: "public/img/buy-comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR",
                    url: "#"
                },
                {
                    img: "public/img/buy-dc-power-visa.svg",
                    text: "DC POWER VISA",
                    url: "#"
                }
            ]
        }
    }
}

</script>

<template>
    <div class="bg">
        <div class="container">

            <ul>
                <li v-for="link in links">
                    <img :src="link.img" alt="link.text">
                    <a :href="link.url">
                        {{ link.text }}
                    </a>
                </li>
            </ul>

        </div>
    </div>
</template>




<style lang = 'scss' scoped>
@use '../Styles/partials/_variables.scss' as *;
@use '../Styles/partials/mixins' as *;

.container {
    width: 1170px;
    margin: 0 auto;
}

.bg {
    background-color: rgb(31 116 224);
    padding: 30px 0;
}


img {
    width: 40px;
    height: 40px;
}


ul{
    @include center;

    li {
    text-decoration: none;
    list-style-type: none;
    @include center;
    margin-left: 80px;

    a {
        text-decoration: none;
        color: white;
        margin-left: 10px;
    }
}
}

</style>
