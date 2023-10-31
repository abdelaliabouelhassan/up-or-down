<template>
    <section class=" w-full h-full relative">
        <!--  -->
        <div class=" w-full relative">
            <img src="images/up-or-down/hero.webp" class=" w-full  h-[50.9375rem] sm:h-[51.3125rem] lg:h-[69.313rem]  object-cover" alt="hero">
            <div class="  w-full h-full  absolute top-[6rem] sm:top-[8rem] lg:top-[12.8rem] left-0">
                <div class="max-w-[32.90744rem]  mx-auto flex flex-col items-center space-y-0 sm:space-y-5">
                    <p class=" text-white font-inter font-extrabold text-[2.25538rem] sm:text-[5rem] text-center leading-[2rem] sm:leading-[4.6rem] relative z-20  ">
                        <span>Up</span> <span class=" text-[1.12769rem] sm:text-[2.5rem]">or</span>
                        <br>
                        <span class=" pl-5">Down</span>
                   </p>
                  <p class=" text-white font-inter text-[0.56381rem] sm:text-xl font-medium relative z-20 lg:pt-14 pt-4 sm:pt-0  ">
                    Bet on the price of bitcoin going up or down
                  </p>

                  <div class=" w-full flex flex-col items-center space-y-0">
                    <div class=" relative z-20">
                        <img src="/images/up-or-down/compgrp.png" class=" w-full h-full object-cover" alt="compgrp">
                    </div>

                    <div class=" relative w-full flex flex-col items-center sm:space-y-2 ">
                        <div class=" w-[22.75rem] h-[5rem] sm:w-[34rem] sm:h-[16rem] absolute -top-[1rem] sm:-top-[6rem]" style="border-radius: 24.9375rem;background: linear-gradient(180deg, #FF5C5C 0%, #F00 100%);filter: blur(50px);flex-shrink: 0;"> </div>
                        <button class=" m-auto relative font-inter text-center rounded-lg w-full hover:rounded-3xl duration-200 text-white text-[1.07556rem] sm:text-[1.76606rem] font-bold bg-primary max-w-[19.87213rem] sm:max-w-[20.49706rem] h-[2.79063rem] sm:h-[4.58231rem]">Connect Wallet</button>
                        <p class=" font-inter text-[0.42288rem] sm:text-[0.9375rem] font-normal text-white relative pt-2 sm:pt-0">
                            no wallet? <a href="" class=" underline hover:text-primary duration-200">Register here</a>
                        </p>
                    </div>
                  </div>
                </div>

                <div class=" w-full flex pt-4 lg:pt-5 relative z-20 ">
                    <img class=" m-auto w-full lg:max-w-[71.8125rem] max-w-[37.52375rem] md:max-w-[58.18581rem] hidden sm:block" src="/images/up-or-down/chart.png"  alt="">
                       <img class=" m-auto w-full h-[32.6875rem]  max-w-[22.75rem]  sm:hidden" src="/images/up-or-down/chart-mobile.png"  alt="">
                </div>
            </div>
        </div>
        <div class=" w-full h-[5rem]  absolute bottom-0 left-0" style="background: linear-gradient(0deg, #11161C 0%, rgba(81, 115, 156, 0.00) 14.7%);"></div>
    </section>
</template>