<template>
    <section class=" w-full h-full relative">
        <!--  -->
        <div class=" w-full relative">
            <img src="/images/up-or-down/hero.webp" class=" w-full  h-[50.9375rem] sm:h-[51.3125rem] lg:h-[69.313rem]  object-cover" alt="hero">
            <div class="  w-full h-full  absolute top-[6rem] sm:top-[8rem] lg:top-[12.8rem] left-0">
                <div   class="max-w-[32.90744rem]  mx-auto flex flex-col items-center space-y-0 sm:space-y-5">
                    <p :class="{'invisible':!show}" class=" text-white font-inter font-extrabold text-[2.25538rem] sm:text-[5rem] text-center leading-[2rem] sm:leading-[4.6rem] relative z-20  ">
                        <span>Up</span> <span class=" text-[1.12769rem] sm:text-[2.5rem]">or</span>
                        <br>
                        <span class=" pl-5">Down</span>
                    </p>
                  <p class=" text-white font-inter text-xs sm:text-xl font-medium relative z-20 lg:pt-14 pt-4 sm:pt-0  ">
                    Bet on the price of bitcoin going up or down
                  </p>

                  <div class=" w-full flex flex-col items-center space-y-0">
                    <div class=" relative z-20">
                        <img src="/images/up-or-down/compgrp.png" class=" w-full h-full object-cover" alt="compgrp">
                    </div>

                    <div class=" relative w-full flex flex-col items-center sm:space-y-2 ">
                        <div class=" w-[22.75rem] h-[5rem] sm:w-[34rem] sm:h-[16rem] absolute -top-[1rem] sm:-top-[6rem]" style="border-radius: 24.9375rem;background: linear-gradient(180deg, #FF5C5C 0%, #F00 100%);filter: blur(50px);flex-shrink: 0;"> </div>
                        <button class=" m-auto relative font-inter text-center rounded-lg w-full hover:rounded-3xl duration-200 text-white text-[1.07556rem] sm:text-[1.76606rem] font-bold bg-primary max-w-[19.87213rem] sm:max-w-[20.49706rem] h-[2.79063rem] sm:h-[4.58231rem]">Connect Wallet</button>
                        <p class=" font-inter text-[0.9375rem] font-normal text-white relative pt-2 sm:pt-0">
                            no wallet? <a href="javascript:void(0)" @click="SignUp" class=" underline hover:text-primary duration-200">Register here</a>
                        </p>
                    </div>
                  </div>
                </div>

                <div class=" w-full flex px-4 pt-20 md:pt-10 lg:pt-20 relative z-20 ">
                   <div class=" m-auto w-full rounded-xl lg:max-w-[71.8125rem] max-w-[37.52375rem] md:max-w-[58.18581rem] h-[51.24806rem]">
                        <Games />
                   </div>
                </div>
            </div>
        </div>

        <Signup ref="SignupRef" />
    </section>
</template>



<script setup>
import Games from "@/components/UI/Games.vue";
import Signup from "@/components/UI/Signup.vue";
 const show = ref(false);
 const SignupRef = ref(null)
 const SignUp = () => {
   SignupRef.value.open();
 }

 onMounted(() => {
   setTimeout(() => {
     show.value = true;
   }, 1000);
 });
</script>