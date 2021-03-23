<template>
  <div class="mlWrapper">
    <meme
      :image="'OH-Wahlkampf.jpg'"
      :text="'ÖH-Wahlkampf (wichtige Vertretungsarbeit) statt Covid-Maßnahmen'"
    />

    <!-- 
    
    Neue Memes hier unter diesem Kommentar einfügen! 
    Beim Text wird automatisch ein 'Erreicht: ' davor eingefügt 

    Wie geht das? siehe bereits bestehende memes...
    
    -->
    <meme
      :image="'VielUmgesetzt.png'"
      :text="'[@blondie3: hier bilduntershift einfügen]'"
    />
    <meme
      :image="'Punschrezept.png'"
      :text="'Euer TAG wünscht euch viel Spaß beim stilvollen Genießen'"
    />
    <meme
      :image="'0NeueKlausuren.png'"
      :text="'Endlich wieder befriedigende Credits!'"
    />
    <meme
      :image="'FroheOsternTAG.png'"
      :text="'Im Zuge von sinnvoller Vertretungsarbeit Oster-Flyer verteilt'"
    />
    <meme :image="'RIP_Steuerrecht.png'" :text="'Steuerrecht beseitigt'" />
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
