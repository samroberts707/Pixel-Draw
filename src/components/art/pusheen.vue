<template>
    <div id="pusheen"></div>
</template>

<script>
export default {
  name: 'Pusheen'
}
</script>

<style lang="scss" scoped>
$size: 10px;

$t: transparent;
$black: #000;
$gray: #cdc9cf;
$dkgray: #a09da1;
$pink: #ffa6ed;
$cat: (
  ($t, $t, $t, $black, $t, $t, $t, $t, $t, $t, $black),
  ($t, $t, $black, $gray, $black, $t, $t, $t, $t, $black, $gray, $black),
  ($t, $t, $black, $gray, $dkgray, $black, $black, $black, $black, $dkgray, $gray, $black, $t, $t, $t, $t, $t, $t, $t, $t, $black, $black),
  ($t, $black, $dkgray, $gray, $gray, $dkgray, $dkgray, $gray, $dkgray, $gray, $gray, $dkgray, $black, $t, $t, $t, $t, $t, $t, $black, $gray, $gray, $black),
  ($t, $black, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $black, $t, $t, $t, $t, $t, $t, $black, $gray, $gray, $black),
  ($black, $dkgray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $dkgray, $black, $black, $black, $black, $t, $t, $t, $black, $dkgray, $black),
  ($black, $gray, $gray, $black, $gray, $gray, $black, $gray, $gray, $black, $gray, $gray, $gray, $dkgray, $gray, $dkgray, $gray, $black, $t, $t, $black, $gray, $black),
  ($black, $gray, $pink, $gray, $gray, $black, $gray, $black, $gray, $gray, $pink, $gray, $gray, $dkgray, $gray, $dkgray, $gray, $gray, $black, $black, $black, $dkgray, $black),
  ($black, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $black, $gray, $black),
  ($black, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $black, $gray, $black),
  ($black, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $black),
  ($black, $dkgray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $black),
  ($black, $dkgray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $black),
  ($black, $dkgray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $dkgray, $black),
  ($t, $black, $dkgray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $gray, $dkgray, $black),
  ($t, $t, $black, $dkgray, $gray, $dkgray, $dkgray, $gray, $dkgray, $gray, $gray, $gray, $dkgray, $gray, $dkgray, $dkgray, $gray, $dkgray, $black),
  ($t, $t, $t, $black, $gray, $black, $black, $gray, $black, $black, $black, $black, $black, $gray, $black, $black, $gray, $black),
  ($t, $t, $t, $black, $black, $t, $t, $black, $black, $t, $t, $t, $black, $black, $t, $t, $black, $black)
);

#pusheen {
  position: relative;
  width: calc(23 * #{$size});
  height: calc(18 * #{$size});
  margin: 1rem;
  &::after {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: $size;
    height: $size;
    box-shadow:
    pixelize($cat, $size);
  }
}
</style>
