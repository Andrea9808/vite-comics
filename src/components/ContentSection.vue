<script>

export default {
    name: "ContentSection",
}

</script>

<template>
    <div class="bg">

        <div class="container">

            <h1 class="title"> - - > CONTENT GOES HERE </h1>

        </div>
    </div>
</template>




<style lang = 'scss' scoped>
@use '../Styles/partials/_variables.scss' as *;
@use '../Styles/partials/mixins' as *;

.container {
    max-width: 1170px;
    margin: 30px auto;
    display: flex;
}

.title {
    color: $primary;
}
</style>
