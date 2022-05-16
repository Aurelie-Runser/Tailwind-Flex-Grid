<template>
    <figure class="flex flex-col w-auto h-auto m-4">
        <img
            class="w-full h-48 object-cover rounded-t-lg"
            :src=image
            alt="image d'une maison" />

        <figcaption class="relative flex flex-col p-5 bg-white rounded-b-lg border-2 borer-t-0 border-indigo-100">
            
            <div class="flex flex-col h-24 justify-around ">
                <div class="flex items-center">
                    <div class="pr-1 font-bold text-2xl text-indigo-500">${{price}}</div>
                    <p class="text-xs text-gray-500">/month</p>
                </div>
        
                <h3 class="font-bold text-2xl text-gray-900">{{nom}}</h3>
                <p class=" text-base font-medium text-gray-500">{{adress}}</p>
           </div>

            <separateur/>

            <div class="flex flex-none flex-row justify-between text-xs text-gray-500">
                <div class="w-max">
                    <bed class="h5 w-5 mr-1 inline-block"/>
                    {{bed}} Beds
                </div>
                <div class="w-max">
                    <bath class="h5 w-5 mr-1 inline-block"/>
                    {{bathroom}} Bathrooms
                </div>
                <div class="w-max">
                    <losange class="h5 w-5 mr-1 inline-block"/>
                    {{taille}} m²
                </div>
            </div>

            <div class="absolute top-0 right-0 m-4 p-3 border-2 rounded-full border-indigo-100">
                <heart class="w-5 h-auto"/>
            </div>

        </figcaption>
    </figure>
</template>

<script>
import bed from "./icones/bed.vue";
import bath from "./icones/bath.vue";
import losange from "./icones/losange.vue";
import heart from "./icones/heart.vue";
import separateur from "./separateur.vue";

export default {
 name: "App",
 components: {bed, bath, losange, heart, separateur},
 props:{
     image:{
         type: String,
     },
     price:{
        type: Number,
        default: 0,
     },
     nom:{
         type: String,
         default: "Nom",
     },
     adress:{
         type: String,
         defalut: "Adresse"
     },
     bed:{
         type: Number,
         defalut: "0"
     },
     bathroom:{
         type: Number,
         defalut: "0"
     },
     taille:{
         type: String,
         defalut: "0"
     },
 }
}

</script>
