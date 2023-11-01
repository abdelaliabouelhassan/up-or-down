<template>
    <div class=" w-full ">
        <FirstSectionVue />
       <div class=" w-full pt-[5rem] sm:pt-[10rem] md:pt-[25.5rem]">
         <SecondSectionVue />
       </div>
    </div>
</template>


<script setup>
 import FirstSectionVue from "@/components/partials/sections/up-or-down/FirstSection.vue";
 import SecondSectionVue from "@/components/partials/sections/up-or-down/SecondSection.vue";
</script>