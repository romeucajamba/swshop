<script setup lang="ts">
import InformationsComponent from './InformationsComponent.vue';
import FooterComponent from './FooterComponent.vue';
defineProps<{
  msg: string
}>()

</script>

<template>
  <main class="flex flex-col w-screen h-[255vh] bg-green-600">
   
  <section class="flex flex-row bg-[#fff] w-screen h-[45rem]">

    <div class="absolute z-20 flex flex-col space-y-4 pt-2 w-[20rem]
                 h-[8rem] bg-[#FFCFCF] rounded-[0.5rem] border-solid
                ml-[37.8%] mt-[5%] animate-pulse shadow-xl"
      >
        <h3 class="text-[#373645] font-semibold text-[1.8rem] pl-6">{{ msg }}</h3>
        <p class="text-[#B79AA1] pl-6">You can get up to 10 percent discount <br/> from here!</p>
    </div>

    <div class="bg-[#FFF8CE] z-10 w-[46rem] space-y-4">

      <img alt="Figura" class="z-20 w-[30rem] h-[12rem] mt-[10%] ml-[3%] animate-bounce" src="@/assets/figura.png" /> 

      <div class="pl-16 mt-[10%] space-y-6">
        <h2 class="text-7xl font-bold">Explore our <br/> new colections</h2>

            <p> Every man needs a good solid watch. I onw many
                watches, but this on is <br/>usually the one my wrist.
                It's help you track you all day steps, colories <br/> 
                consumptions, distance traveled & heart rate.
          </p>
      </div>

      <div class="pl-16 space-x-6">
          <button type="submit" class="bg-[#00D77F] text-[#fff]
             hover:cursor-pointer hover:bg-[#fff] hover:text-[#00D77F]
             rounded-md font-semibold w-[9rem] h-[4rem]">
             Order now
          </button>

          <button type="submit" class="text-[#000] hover:cursor-pointer 
                hover:text-[#FFF] rounded-md font-semibold w-[9rem] h-[4rem] border-2 border-[#000]">
                Explore more
          </button>

      </div>
    </div>

    <div class="bg-[#091B26] w-[46rem] felx flex-col z-10">

      <div class="bg-[#E4EBAC] w-[8rem] h-[8rem] rounded-xl 
                    flex flex-col text-center p-3  ml-[35%] mt-[5%] absolute z-40">

          <svg xmlns="http://www.w3.org/2000/svg" fill="true" 
              viewBox="0 0 24 24" strokeWidth={1.5} stroke="currentColor" 
              className="w-6 h-6">
            <path strokeLinecap="round" strokeLinejoin="round" 
                  d="M2.25 15a4.5 4.5 0 0 0 4.5 4.5H18a3.75 3.75 
                      0 0 0 1.332-7.257 3 3 0 0 0-3.758-3.848 5.25 
                      5.25 0 0 0-10.233 2.33A4.502 4.502 0 0 0 2.25 15Z" />
          </svg>

        <span class="font-bold text-[1.3rem]">20ºF</span>
        <span class="font-semibold text-[0.9rem]">Cloudy</span>

      </div>
      <img alt="Watch" class="w-[35rem] h-[35rem]
              mt-[14%] ml-[8%] z-10" src="@/assets/smart9-removebg-preview.png" /> 
    </div>
  </section>

    <div class="absolute z-40 w-[12rem] h-[15rem] ml-[47%] 
              bg-[#FFFFFF] rounded-2xl flex flex-col 
              mt-[39%] shadow-2xl">

        <img alt="Watch" class="w-[10rem] h-[10rem]
              mt-[14%] ml-[8%] z-10" src="@/assets/steps.png" />
        
    </div>

    <InformationsComponent/>
    <FooterComponent />
  </main>
</template>

<style scoped>
.icon {
  width: 3rem;
  height: 3rem;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
