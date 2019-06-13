<template>
  <footer>
    <p>Made by <a href="https://github.com/samroberts707" target="_blank">Sam Roberts</a></p>
  </footer>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<style lang="scss" scoped>
footer {
  display: block;
  width: 100vw;
  padding: 0 5%;
  p {
    text-align: center;
    padding: 30px 0;
    border-top: 1px solid rgba($color: #FFF, $alpha: 0.5);
  }
}
</style>
