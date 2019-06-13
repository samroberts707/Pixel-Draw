<template>
  <nav>
    <div class="logo">
      <img src="https://via.placeholder.com/75" id="logo" >
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navigation"
};
</script>

<style lang="scss" scoped>
nav {
  display: grid;
  grid-template-columns: 90%;
  width: 100vw;
  div.logo {
    margin-left: 5%;
    padding: 20px 0;
    img#logo {
      display: block;
    }
  }
}
</style>
