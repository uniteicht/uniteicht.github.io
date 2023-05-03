<template>
  <div class="mlWrapper">    
    <!--    
    Neue Memes hier unter diesem Kommentar einfügen! 
    Beim Text wird automatisch ein 'Erreicht: ' davor eingefügt 

    Wie geht das? siehe bereits bestehende memes...    
    -->
    <meme image="horoskop.png"> DEIN <i>völlig individuelles</i> Horoskop </meme>
    <meme image="service.png"> Für DICH nur den besten Service! Von MIR! Deine Fanessa &lt;3 </meme>
    <meme image="firstblood.jpg"> First Blood! Die Ersten werden die Letzten sein! Nein, warte... wie ging das? </meme>
    <meme image="tim.jpg"> SUCHE noch die Unterschriften mit dem etwas kleineren "G", und die, wo das zweite "s" fehlt. Kann gerne auch tauschen! (Bei meinen ist leider ein Fehler, "V" statt "F"). Die anderen 498 Teile der Sammlung habe ich schon.</meme>
    <meme image="uniteicht.png"> lol </meme>
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
