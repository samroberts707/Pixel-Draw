<template>
    <div id="mario"></div>
</template>

<script>
export default {
  name: 'Mario'
}
</script>

<style lang="scss" scoped>
$size: 10px;

$t: transparent;
$black: #000000;
$red: #FF0000;
$blue: #0000FF;
$skin: #FF9900;
$brown: #783F04;

$mario: (
  ($t,$t,$t,$red,$red,$red,$red,$red),
  ($t,$t,$red,$red,$red,$red,$red,$red,$red,$red,$red),
  ($t,$t,$brown,$brown,$brown,$skin,$skin,$brown,$skin),
  ($t,$brown,$skin,$brown,$skin,$skin,$skin,$brown,$skin,$skin,$skin),
  ($t,$brown,$skin,$brown,$brown,$skin,$skin,$skin,$brown,$skin,$skin,$brown),
  ($t,$brown,$brown,$skin,$skin,$skin,$skin,$brown,$brown,$brown,$brown),
  ($t,$t,$t,$skin,$skin,$skin,$skin,$skin,$skin,$skin),
  ($t,$t,$red,$red,$blue,$red,$red,$red,$red),
  ($t,$red,$red,$red,$blue,$red,$red,$blue,$red,$red,$red),
  ($red,$red,$red,$red,$blue,$blue,$blue,$blue,$red,$red,$red,$red),
  ($skin,$skin,$red,$blue,$skin,$blue,$blue,$skin,$blue,$red,$skin,$skin),
  ($skin,$skin,$skin,$blue,$blue,$blue,$blue,$blue,$blue,$skin,$skin,$skin),
  ($skin,$skin,$blue,$blue,$blue,$blue,$blue,$blue,$blue,$blue,$skin,$skin),
  ($t,$t,$blue,$blue,$blue,$t,$t,$blue,$blue,$blue),
  ($t,$brown,$brown,$brown,$t,$t,$t,$t,$brown,$brown,$brown),
  ($brown,$brown,$brown,$brown,$t,$t,$t,$t,$brown,$brown,$brown,$brown)
);

#mario {
  position: relative;
  width: calc(12 * #{$size});
  height: calc(16 * #{$size});
  margin: 1rem;
  &::after {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: $size;
    height: $size;
    box-shadow:
    pixelize($mario, $size);
  }
}
</style>
