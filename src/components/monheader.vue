<template>
    <nav class="flex items-center justify-between w-full h-16 lg:h-24 p-7 bg-white border-b-2 border-indigo-100">
        <router-link to="/" class="flex items-center justify-between w-32 h-12 p-1">
            <home/>
            <p class="font-inter text-xl font-bold">Estatery</p>
        </router-link>

        <div class="hidden flex-auto lg:flex">
            <ul class="flex flex-auto items-center justify-evenly mr-32">
                <li><router-link to="/" class="font-inter text-base font-medium">Rent</router-link></li>
                <li><router-link to="/" class="font-inter text-base font-medium">Buy</router-link></li>
                <li><router-link to="/" class="font-inter text-base font-medium">Sell</router-link></li>
                <li><router-link to="/" class="font-inter text-base font-medium">Manage Property<fleche class="inline ml-1"/></router-link></li>
                <li><router-link to="/" class="font-inter text-base font-medium">Resources<fleche class="inline ml-1"/></router-link></li>
            </ul>
            <div class="flex w-56 flex-shrink justify-between">
                <login/>
                <signUp/>
            </div>
        </div>

        <button class="relative z-50 text-xl lg:hidden">
            <menuburger/>
            <span class="sr-only">Menu</span>
        </button>

    </nav>
</template>

<script>
import home from "./icones/home.vue";
import menuburger from "./icones/menuburger.vue";
import fleche from "./icones/flecheBasBlack.vue";
import login from "./login.vue";
import signUp from "./signUp.vue";


export default {
 name: "App",
 components: {home, menuburger, fleche, login, signUp},

}
</script>

<!--

        -->