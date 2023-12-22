<script>
export default {
    name: "ComicsSection",

    props: {
        details: Object,
    }
}


</script>

<template>
    <div class="card">
        <img :src="details.thumb" :alt="details.series">
        <div>
            <span>{{ details.series }}</span>
            <span class="price">{{ details.price }}</span>
        </div>
        <div>
            <span>Tipo di fumetto: {{ details.type }}</span>
        </div>
    </div>
</template>




<style lang = 'scss' scoped>
@use '../Styles/partials/_variables.scss' as *;
@use '../Styles/partials/mixins' as *;

.card {
    width: calc(100% / 6);
    padding: 40px 10px;
    color: $primary;

    img {
        width: 100%;
        height: 100%;
    }

    .price{
        margin-left: 15px;
        background-color: red;
    }
}
</style>
