<script>
import Products from "./components/Products.vue";
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    Products,
    Header,
    Footer
  },
};
</script>

<template>
  <div>
    <Header/>
    <Products />
    <Footer />

  </div>
</template>

<style>

body {
  background-color: sandybrown; 
  color: black; 
}

</style>