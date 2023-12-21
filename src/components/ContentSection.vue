<script>

export default {
    name: "ContentSection",
}

</script>

<template>

    <div class="bg">

        <h1 class="title"> - - > CONTENT GOES HERE </h1>

    </div>

</template>




<style lang = 'scss' scoped>
@use '../Styles/partials/_variables.scss' as *;
@use '../Styles/partials/mixins' as *;

.bg{
    height: 72px;
    @include around;
}

.title{
    color: $primary;;
}

</style>
