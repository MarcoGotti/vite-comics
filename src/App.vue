<script>
import AppHeader from "./components/AppHeader.vue";
import AppMainTop from "./components/AppMainTop.vue";
import AppMainBottom from "./components/AppMainBottom.vue";
import AppFooterTop from "./components/AppFooterTop.vue";
import AppFooterBottom from "./components/AppFooterBottom.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMainTop,
    AppMainBottom,   
    AppFooterTop,
    AppFooterBottom 
  }
}
</script>

<template>

  <AppHeader></AppHeader>
  
  <main>

    <AppMainTop></AppMainTop>
    <AppMainBottom></AppMainBottom>

  </main>

  <footer>

    <AppFooterTop></AppFooterTop>
    <AppFooterBottom></AppFooterBottom>
    


  </footer>

</template>

<style>

</style>
