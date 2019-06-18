<template>
  <div class="home">
    <div class="logo">
      <h1>Pixel Draw</h1>
      <h2>The pure CSS Pixel Art collection</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home"
};
</script>

<style lang="scss" scoped>
div.home {
  display: block;
  padding: 5%;
  div.logo {
    h1 {
      font-size: 3vw;
      text-align: center;
      font-family: 'Press Start 2P', cursive;
    }
    h2 {
      font-size: 2vw;
      text-align: center;
      margin-top: 30px;
    }
  }
}
</style>
