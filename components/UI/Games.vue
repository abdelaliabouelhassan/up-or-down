<template>
  <div class="w-full h-full relative">
    <div class=" bg-[#1B2128] rounded-t-[0.625rem] px-2 pt-2 w-full flex items-center justify-between max-w-[14.125rem] absolute -top-16 right-1">
        <div :class="{'bg-[#0E1824]':selectedGame === 0}" @click="selectGame(0)" class=" duration-200 w-[3.4375rem] h-[3.8125rem] rounded-t-[0.625rem] flex cursor-pointer">
            <img src="/images/up-or-down/updown.png" alt="" class=" m-auto">
        </div>
         <div :class="{'bg-[#0E1824]':selectedGame === 1}" @click="selectGame(1)"  class=" duration-200  w-[3.4375rem] h-[3.8125rem] rounded-t-[0.625rem] flex cursor-pointer">
            <img src="/images/up-or-down/coming-soojn1.png" alt="" class=" m-auto">
        </div>
         <div :class="{'bg-[#0E1824]':selectedGame === 2}" @click="selectGame(2)"  class="duration-200   w-[3.4375rem] h-[3.8125rem] rounded-t-[0.625rem] flex cursor-pointer">
            <img src="/images/up-or-down/coming-soojn2.png" alt="" class=" m-auto">
        </div>
         <div :class="{'bg-[#0E1824]':selectedGame === 3}" @click="selectGame(3)"  class=" duration-200  w-[3.4375rem] h-[3.8125rem] rounded-t-[0.625rem] flex cursor-pointer">
            <img src="/images/up-or-down/coming-soojn3.png" alt="" class=" m-auto">
        </div>
    </div>
    <div class=" w-full h-full relative" v-if="selectedGame === 0">
        <iframe 
        class="overflow-hidden rounded-xl"
        width="100%"
        height="100%"
        src="https://upordown.bitbloxrgs.com?id=17&subscriptionKey=PIoEaXgGypHeBRTDhDkrsBUCBhCoXkcFoIXspGqUjRPz&token=test1"
        title=""
        style="border: unset"
        >
        </iframe>
    </div>
    <div class=" w-full h-full relative" v-if="selectedGame === 1">

           <img class="  w-full h-full hidden sm:block" src="/images/up-or-down/chart.png"  alt="">
           <img class="  w-full h-full   sm:hidden" src="/images/up-or-down/chart-mobile.png"  alt="">
    </div>
     <div class=" w-full h-full relative" v-if="selectedGame === 2">

    </div>
     <div class=" w-full h-full relative" v-if="selectedGame === 3">

    </div>
  </div>
</template>


<script setup>
 const selectedGame = ref(0)

 const selectGame = (index) => {
    selectedGame.value = index
 }
</script>