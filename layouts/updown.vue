<template>
    <div class=" w-full bg-[#11161C] h-full text-white overflow-hidden">
        <div class=" w-full px-4 xl:px-0 absolute z-50 flex py-5">
            <div class=" mx-auto md:pt-5 max-w-[87.875rem] w-full">
                <Header  />
            </div>
        </div>

        <div class=" w-full">
             <slot />
        </div>
         <!-- <Footer /> -->
    </div>
</template>


<script setup>
    import Header from "@/components/partials/Header.vue"
    
</script>