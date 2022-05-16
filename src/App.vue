<template>
  <div class="bg-indigo-25">
    <monheader/>
    
    <search/>

    <div class="grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(22rem,1fr))] max-w-7xl m-auto">
      <card image="public/maison1.jpg"
            price="2,700"
            nom="Beverly Springfield"
            adress="2821 Lake Sevilla, Palm Harbor, TX "
            bed="4"
            bathroom="2"
            taille="6x7.5"/>

      <card image="public/maison2.jpg"
            price="2,095"
            nom="Palm Harbor"
            adress="2699 Green Valley, Highland Lake"
            bed="4"
            bathroom="2"
            taille="6x7"/>

      <card image="public/maison3.jpg"
            price="4,550"
            nom="Faulkner Ave"
            adress="909 Woodland St, Michigan, IN"
            bed="4"
            bathroom="3"
            taille="8x10"/>

      <card image="public/maison4.jpg"
            price="4,650"
            nom="St. Christal"
            adress="210 US Highway, HighlandLake, FL"
            bed="4"
            bathroom="2"
            taille="6x7.5"/>

      <card image="public/maison5.jpg"
            price="3,100"
            nom="Cover Red"
            adress="243 CurlewRoad, PalmHarbor, TX"
            bed="4"
            bathroom="2"
            taille="6x7.5"/>

      <card image="public/maison6.jpg"
            price="4,800"
            nom="Tarpon Bay"
            adress="103 Lake Shores, Michigan, IN"
            bed="4"
            bathroom="2"
            taille="6x7.5"/>
    </div>

    <monfooter/>
    
  </div>  
</template>

<script >
import monheader from "./components/monheader.vue";
import search from "./components/search.vue";
import card from "./components/card.vue";
import monfooter from "./components/monfooter.vue";
import boutton from "./components/boutton.vue";
import titre from "./components/titre.vue";
import separateur from "./components/separateur.vue";

export default {
 name: "App",
 components: {monheader, search, card, monfooter, boutton, titre, separateur},
};

</script>
