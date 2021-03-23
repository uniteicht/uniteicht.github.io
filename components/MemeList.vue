<template>
  <div class="mlWrapper">
    <meme :image="'RIP_Steuerrecht.png'" :text="'Mein Text'" />
  </div>
</template>

<script>
import Meme from "./Meme.vue";
export default {
  components: { Meme },
};
</script>

<style>
.mlWrapper {
  width: 100%;
}
</style>
