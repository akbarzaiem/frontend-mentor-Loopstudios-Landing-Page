<template>
  <div class="container">
    <Header />
    <Hero-vr />
    <Creation />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import HeroVr from "./components/Hero-vr.vue";
import Creation from "./components/Creation.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    HeroVr,
    Creation,
    Footer,
  },
};
</script>

<style scoped>
.container {
  height: 100%;
  width: 100%;
  left: 0;
  top: 0;
  overflow-y: scroll;
  position: fixed;
}
</style>
