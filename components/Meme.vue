<template>
  <div class="meme">
    <img class="meme-img" :src="'/meme/' + image" />
    <h3 class="meme-desc">Erreicht: {{ text }}</h3>
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
  width: 100%;
  border: 1px solid;
  text-align: center;
  margin-bottom: 20px;
}

.meme-img {
  max-width: 100%;
  max-height: 700px;
  padding-bottom: 15px;
}
</style>
