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
@import url('https://fonts.googleapis.com/css?family=Montserrat:400,500,600|Press+Start+2P&display=swap');
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  border: 0;
	font-size: 100%;
	font: inherit;
	vertical-align: baseline;
}
:root {
  --black: #222;
  --blue: #BAE1FF;
  --green: #BAFFC9;
  --yellow: #FFFFBA;
  --orange: #FFDFBA;
  --pink: #FFB3BA;
}
body {
  background-color: var(--orange);
  p, li, a, h1, h2, h3, h4, h5, h6 {
    font-family: 'Montserrat', sans-serif;
    color: var(--black);
  }
}
</style>
