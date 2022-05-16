<template>
    <div class="w-full bg-white">
        <div class="py-12">
            <div class="flex items-center justify-between w-32 h-12 mx-8 p-1">
                <home/>
                <p class="font-inter text-xl font-bold">Estatery</p>
            </div>

        <div class="grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(10rem,1fr))] max-w-xl p-4 m-auto">
                <navFooter title="Sell a home"
                txt1="Request an offer"
                txt2="Pricing"
                txt3="Reviews"
                txt4="Stories" />
 
                <navFooter title="Buy a home"
                txt1="Buy"
                txt2="Finance" />
 
                <navFooter title="Buy, rent and sell"
                txt1="Buy & sell properties"
                txt2="Rent home"
                txt3="Builder trade-up" />
 
                <navFooter title="Terms & privacy"
                txt1="Trust & Safety"
                txt2="Terms of Service"
                txt3="Privacy Policy" />
 
                <navFooter title="About"
                txt1="Company"
                txt2="How it works"
                txt3="Contact"
                txt4="Investors" />
 
                <navFooter title="Resources"
                txt1="Blog"
                txt2="Guides"
                txt3="FAQ"
                txt4="Help Center" />
 
            </div>
        </div>

        <div class="text-center h-36 -my-16">
            <separateur class="my-10"/>
            <p class="font-inter text-gray-500">©2021 Estatery. All rights reserved</p>
            <div class="flex justify-evenly w-auto m-8">
                <facebook/>
                <insta/>
                <twitter/>
                <linkedin/>
            </div>
        </div>
        
    </div>
</template>

<script>
import home from "./icones/home.vue";
import facebook from "./icones/facebook.vue";
import insta from "./icones/insta.vue";
import twitter from "./icones/twitter.vue";
import linkedin from "./icones/linkedin.vue";
import navFooter from "./navFooter.vue";
import separateur from "./separateur.vue";

export default {
name: "App",
components: {home, facebook, insta, twitter, linkedin, navFooter, separateur },

}
</script>