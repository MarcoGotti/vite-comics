<script>
import AppHeader from "./components/AppHeader.vue";
import AppMainTop from "./components/AppMainTop.vue";
import AppMainBottom from "./components/AppMainBottom.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMainBottom,
    AppMainTop,
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

    <div id="footer_top"></div>
    <div id="footer_bottom"></div>

  </footer>

</template>

<style>

</style>
