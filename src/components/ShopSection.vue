<script>

export default {
    name: "ShopSection",

    data(){
        return{
            links:[
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

        <ul>
            <li v-for="link in links">
                <img :src="link.img" alt="link.text">
                <a :href="link.url">
                  {{ link.text }}  
                </a>
            </li>
        </ul>

    </div>

</template>




<style lang = 'scss' scoped>
@use '../Styles/partials/_variables.scss' as *;
@use '../Styles/partials/mixins' as *;

.bg{
    background-color: rgb(31 116 224);
    padding: 30px 0;
    @include center;
}


img{
    width: 40px;
    height: 40px;
}

li {
    text-decoration: none;
    list-style-type: none;
    display: inline-block;
    padding-right: 50px;
  
    a {
        text-decoration: none;
        color: white;
        margin-left: 10px;
    }
}

</style>
