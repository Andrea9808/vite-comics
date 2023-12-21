<script>
  import HeaderSection from './components/HeaderSection.vue'

  export default {
    components:{
      HeaderSection,
    }
  }
</script>

<template>
  <header>
    <HeaderSection/>
  </header>
  
</template>

<style lang = 'scss'>
  @use './Styles/general.scss' as *;
  @use './Styles/partials/_variables.scss' as *;
</style>
