<template>
  <div class="home">
    <div class="logo">
      <h1>Pixel Draw</h1>
      <h2>The pure CSS Pixel Art collection</h2>
    </div>
    <div class="art-grid">
      <Pusheen></Pusheen>
    </div>
  </div>
</template>

<script>
import Pusheen from '../components/art/pusheen.vue';
export default {
  name: "Home",
  components: {
    Pusheen
  }
};
</script>

<style lang="scss" scoped>
div.home {
  display: block;
  padding: 5%;
  div.logo {
    h1 {
      font-size: 4vw;
      text-align: center;
      font-family: 'Press Start 2P', cursive;
      @media screen and (max-width: 1024px) {
        font-size: 5vw;
      }
      @media screen and (max-width: 768px) {
        font-size: 6vw;
      }
    }
    h2 {
      font-size: 2vw;
      text-align: center;
      margin-top: 30px;
      @media screen and (max-width: 1024px) {
        font-size: 3vw;
      }
      @media screen and (max-width: 768px) {
        font-size: 4vw;
      }
    }
  }
  div.art-grid {
    display: grid;
    grid-template-columns: repeat(4, 25%);
    justify-items: center;
    align-items: center;
    grid-row-gap: 50px;
    padding-top: 50px;
    @media screen and (max-width: 1024px) {
      grid-template-columns: repeat(2, 50%);
    }
    @media screen and (max-width: 768px) {
      grid-template-columns: 1fr;
    }
  }
}
</style>
