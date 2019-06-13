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
  display: block;
  width: 100vw;
  padding: 0 5%;
  div.logo {
    padding: 20px 0;
    img#logo {
      display: block;
    }
  }
}
</style>
