<template>
  <div id="app">
    <Navigation></Navigation>
    <router-view/>
    <Footer></Footer>
  </div>
</template>

<script>
import Navigation from "@/components/Navigation.vue";
import Footer from "@/components/Footer.vue";
export default {
  components: {
    Navigation,
    Footer
  }
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
}
:root {
  --blue: #b0deff;
  --peach: #ffc5a1;
  --orange: #ffd19a;
  --yellow: #fff8a6;
}
</style>
