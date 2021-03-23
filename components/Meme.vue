<template>
  <div class="meme">
    <img :src="'/meme/' + image" />
    <h3>{{ text }}</h3>
  </div>
</template>

<script>
export default {
  props: {
    image: {
      type: String,
    },
    text: {
      type: String,
      default() {
        return "sinnvolle Vertreterarbeit!";
      },
    },
  },
};
</script>

<style>
.meme {
  width: 80%;
  border: 1px solid;
}

img {
  max-height: 500px;
}
</style>
