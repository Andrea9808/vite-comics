<script>
  import HeaderSection from './components/HeaderSection.vue';
  import ContentSection from './components/ContentSection.vue';
  import ShopSection from './components/ShopSection.vue';

  export default {
    components:{
      HeaderSection,
      ContentSection,
      ShopSection
    }
  }
</script>

<template>
  <header>
    <HeaderSection/>
    <ContentSection/>
    <ShopSection/>
  </header>
  
</template>

<style lang = 'scss'>
  @use './Styles/general.scss' as *;
  @use './Styles/partials/_variables.scss' as *;
</style>
