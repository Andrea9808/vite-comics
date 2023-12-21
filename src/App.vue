<script>
  import HeaderSection from './components/HeaderSection.vue';
  import ContentSection from './components/ContentSection.vue';
  import ShopSection from './components/ShopSection.vue';
  import FooterSection from './components/FooterSection.vue';
  import SocialSection from './components/SocialSection.vue';
  

  export default {
    components:{
      HeaderSection,
      ContentSection,
      ShopSection,
      FooterSection,
      SocialSection
    }
  }
</script>

<template>

  <header>
    <HeaderSection/>
  </header>

  <main>
    <ContentSection/>
    <ShopSection/>
  </main>

  <footer>
    <FooterSection/>
    <SocialSection/>
  </footer>
  
</template>

<style lang = 'scss'>
  @use './Styles/general.scss' as *;
  @use './Styles/partials/_variables.scss' as *;

</style>
