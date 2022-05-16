<template>
    <div class="mt-14 w-full h-auto">

        <div class="flex flex-col lg:flex-row">
            <titre class="w-[500] flex-grow text-center lg:text-left">Search properties to rent</titre>

            <div class="flex justify-between items-center lg:w-96 h-12 mx-4 my-8 p-1 bg-white rounded-lg border-2 border-indigo-100 font-inter text-gray-700">
                <p class="inline mx-4">Search with Search Bar</p>
                <flecheBas class="inline w-6 h-6 mx-4 p-1 rounded-full bg-indigo-100"/>
            </div>
        </div>

        <div class="flex justify-between items-center w-auto h-16 mx-4 my-8 p-2 bg-white rounded-lg fton-inter text-gray-500 lg:hidden">
            <p class="mx-4">Search location</p>
            <loupe class="w-11 h-11 p-3 rounded-lg bg-indigo-500"/>
        </div>

        <div class="hidden justify-between m-3 px-8 py-6 rounded-lg bg-white lg:flex">
            <div class="font-inter">
                <p class="text-base font-medium leading-6 text-gray-500">Location</p>
                <p class="text-lg leading-7 font-bold text-gray-900">New York, USA</p>
            </div>
            <div class="font-inter px-8 border-l border-l-indigo-100">
                <p class="text-base font-medium leading-6 text-gray-500">When</p>
                <p class="text-lg leading-7 font-bold text-gray-900">Select Move-in Date</p>
            </div>
            <div class="font-inter px-8 border-l border-l-indigo-100">
                <p class="text-base font-medium leading-6 text-gray-500">Price</p>
                <p class="text-lg leading-7 font-bold text-gray-900">$500-$2,500</p>
            </div>
            <div class="px-8 border-l border-l-indigo-100">
                <searchButton/>
            </div>

        </div>

    </div>
</template>

<script>
import titre from "./titre.vue";
import flecheBas from "./icones/flecheBas.vue";
import loupe from "./icones/loupe.vue";
import searchButton from "./icones/searchButton.vue";

export default {
 name: "App",
 components: {titre, flecheBas, loupe, searchButton},
};
</script>
