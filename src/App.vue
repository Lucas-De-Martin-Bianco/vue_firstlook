<script>
import Header from "./components/Header.vue";
import Products from "./components/Products.vue";
import Footer from "./components/Footer.vue";

export default {
  components: {
    Header,
    Products,
    Footer,
  },
};
</script>

<template>
  <div>
    <Header />
    <Products />
    <Footer />
  </div>
</template>

<style>
  body {
    background-color: grey;
    color:black;
  }
</style>