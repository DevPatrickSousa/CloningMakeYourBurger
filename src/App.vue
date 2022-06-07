<template>
  <Nav-Bar :logo="logo_src" :alt="app_name" />
  <router-view />
  <Footer />
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    NavBar,
    Footer,
  },
  data() {
    return {
      logo_src: "img/logo.png",
      app_name: "make your burger",
    };
  },
};
</script>
<style>
</style>
