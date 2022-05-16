<template>
    <div class="w-40 h-auto my-4 text-sm font-inter">
        <p class="font-bold uppercase mb-4">{{title}}</p>
        <ul class="text-gray-500">
            <li class="text-sm not-italic">{{txt1}}</li>
            <li class="text-sm not-italic">{{txt2}}</li>
            <li class="text-sm not-italic">{{txt3}}</li>
            <li class="text-sm not-italic">{{txt4}}</li>
        </ul>
    </div>
</template>

<script>

export default {
 name: "App",
 props:{
     title:{
         type: String,
     },
     txt1:{
         type: String,
     },
     txt2:{
         type: String,
     },
     txt3:{
         type: String,
     },
     txt4:{
         type: String,
     },
 }
}
</script>
