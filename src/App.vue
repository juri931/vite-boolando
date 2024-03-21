<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Main from "./components/Main.vue";
export default {
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<template>
  <Header />
  <Main />
  <Footer />
</template>

<style lang="scss" scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
