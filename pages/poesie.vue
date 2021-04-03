<template>
  <div class="poesie-wrapper">
    <h1>POSIE-ALBUM</h1>
    <p>
      Zum Poesie-Album: Inspiriert von
      <a href="https://www.instagram.com/p/CMXrs8fjT7c/ " target="blank"
        >diesem genialen Meme</a
      >
      auf dem Instagram-Account einer gewissen "ag.jku.uniteich" hat unsere
      liebe Anastasia begonnen, sich selbst lyrisch auszuleben. Hier eine
      Auswahl ihrer poetischen Ergüsse:
    </p>

    <div class="mlWrapper">
      <meme :achieved="false" image="poesie/OffenerBrief_Poesie.png" />
      <meme :achieved="false" image="poesie/OffenerBrief_Newsletter.png" />
      <meme :achieved="false" image="poesie/OffenerBrief_Blatt.png" />
      <meme :achieved="false" image="poesie/OffenerBrief_Gedanken.png" />
      <meme :achieved="false" image="poesie/OffenerBrief_UniteichtCard.png" />
      <meme :achieved="false" image="poesie/OffenerBrief_Vertretungsarbeit.png" />
      <meme :achieved="false" image="poesie/OffenerBrief_Onlyfans.png" />
    </div>
  </div>
</template>

<style>
</style>

<script>
export default {};
</script>

<style>
.poesie-wrapper {
  width: 80%;
  height: 100%;
  margin: auto;
}

h1 {
  color: black;
}

p {
  font-size: large;
}
</style>
