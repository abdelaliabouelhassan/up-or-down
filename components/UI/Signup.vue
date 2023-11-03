<template>
<div class="relative z-50" aria-labelledby="modal-title" role="dialog" aria-modal="true" v-if="show">
 
  <div class="fixed inset-0 bg-[#000000] bg-opacity-80 transition-opacity"></div>

  <div class="fixed inset-0 z-50 overflow-y-auto">
    <div class="flex min-h-full  h-full items-center justify-center  text-center sm:items-center ">
   
      <div  class="relative transform overflow-y-auto font-inter h-full  sm:rounded-[10px]  w-screen sm:h-auto p-8 bg-[#132932] text-left shadow-xl transition-all sm:my-8  sm:w-full sm:max-w-[449px]">
            <button @click="show = false" class=" cursor-pointer absolute top-4 right-4">
                <svg width="11" height="11" viewBox="0 0 11 11" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path fill-rule="evenodd" clip-rule="evenodd" d="M8.90561 0.674728C9.32148 0.265976 9.99575 0.265976 10.4116 0.674728C10.8275 1.08348 10.8275 1.7462 10.4116 2.15495L6.95361 5.55374L10.5097 9.04896C10.9256 9.45771 10.9256 10.1204 10.5097 10.5292C10.0939 10.9379 9.41959 10.9379 9.00371 10.5292L5.44759 7.03397L1.89147 10.5292C1.47559 10.9379 0.801328 10.9379 0.385453 10.5292C-0.0304215 10.1204 -0.0304212 9.45771 0.385454 9.04896L3.94157 5.55374L0.483557 2.15495C0.0676822 1.7462 0.0676822 1.08348 0.483557 0.674728C0.899432 0.265976 1.5737 0.265976 1.98957 0.674728L5.44759 4.07352L8.90561 0.674728Z" fill="white" fill-opacity="0.5"/>
                </svg>
            </button>

          <div class=" flex flex-col items-center space-y-10">
             <div class=" flex items-center space-x-2">
                <div class="  font-bold text-lg text-center">
                  Register
                </div>
             </div>
           
          </div>

        

          <div  class=" w-full flex flex-col items-center space-y-4 pt-4">
                
              
              

                <div class=" w-full flex flex-col items-start space-y-5">
                    <div class=" flex flex-col items-start space-y-1 w-full">
                        <span class=" text-[#667B83] text-xs font-normal">E-mail  *</span>
                        <input type="text" class=" w-full bg-white rounded-lg h-[2.4rem] p-4 outline-none text-black" placeholder="E-mail">
                    </div>
                     <div class=" flex flex-col items-start space-y-1 w-full">
                        <span class=" text-[#667B83] text-xs font-normal">name</span>
                        <input type="text" class=" w-full bg-white rounded-lg h-[2.4rem] p-4 outline-none text-black" placeholder="Username">
                    </div>
                     <div class=" flex flex-col items-start space-y-1 w-full">
                        <span class=" text-[#667B83] text-xs font-normal">surname</span>
                        <input type="text" class=" w-full bg-white rounded-lg h-[2.4rem]  p-4 outline-none text-black" placeholder="Promo code">
                    </div>
                    <div class=" flex items-center space-x-2">
                        <input class=" w-4 h-4 border border-[#667B83] " type="checkbox">
                        <span class=" text-white font-normal text-xs">I agree with <a href="" class=" underline">Terms and Conditions</a> </span>
                    </div>
                     <div class=" flex items-center space-x-2">
                        <input class=" w-4 h-4 border border-[#667B83]" type="checkbox">
                        <span class=" text-white font-normal text-xs">I confirm that I'm 18 years or older</span>
                    </div>
                </div>
          </div>


          <div class=" flex flex-col items-center space-y-5 pt-10">
                        <button @click="SignUp" class=" md:pr-0 hover:rounded-md cursor-pointer text-white font-bold font-inter text-xs bg-primary rounded-sm max-w-[6.839rem]  w-full h-[2.76rem]  text-center hover:bg-opacity-75 duration-300">Sign Up</button>
          </div>
      </div>
    </div>
  </div>
</div>

</template>


<script setup>
 import PromotionCard from "@/components/UI/PromotionCard.vue"

 const show = ref(false)

 const open = () => {
    show.value = true
 }


 const SignUp = () => {
    show.value = false
 }



 defineExpose({
    open
 })


</script>
