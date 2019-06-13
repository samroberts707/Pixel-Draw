<template>
  <div class="home">
    <div class="logo">
      <img src="https://via.placeholder.com/1000" id="logo">
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
    img {
      display: block;
      margin: auto;
      width: 33vw;
    }
    h2 {
      font-size: 2vw;
      text-align: center;
      margin-top: 30px;
    }
  }
}
</style>
