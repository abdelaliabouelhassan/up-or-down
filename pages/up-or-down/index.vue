<template>
    <div class=" w-full ">
        <FirstSection />
       <div class=" w-full pt-[29rem]  sm:pt-[40rem] lg:pt-[30.5rem]">
         <SecondSection />
       </div>
       <ThirdSection />
    </div>
</template>


<script setup>
 import FirstSection from "@/components/partials/sections/up-or-down/FirstSection.vue";
 import SecondSection from "@/components/partials/sections/up-or-down/SecondSection.vue";
 import ThirdSection from "@/components/partials/sections/up-or-down/ThirdSection.vue";
</script>