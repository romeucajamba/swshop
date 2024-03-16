<script setup lang="ts">

defineProps<{
  msg: string
}>()

</script>

<template>
  <main>
   
  <section class="flex flex-row bg-[#fff] w-screen h-[50rem]">

    <div class="absolute z-20 flex flex-col space-y-4 p-2 w-[20rem]
                 h-[8rem] bg-[#FFCFCF] rounded-[0.5rem] border-solid
                ml-[30%]"
      >
        <h3 class="text-[#373645] font-semibold text-[1.8rem] pl-6">{{ msg }}</h3>
        <p class="text-[#B79AA1] pl-6">You can get up to 10 percent discount from here!</p>
    </div>

    <div class="bg-[#FFF8CE] z-10 w-[46rem]">

      <h2>Explore our new colections</h2>

      <p>Every man needs a good solid watch. I onw many
         watches, but this on is <br/>usually the one my wrist.
         It's help you track you all day steps, colories <br/> 
        consumptions, distance traveled & heart rate.
      </p>
      <div>
          <button type="submit" class="bg-[#00D77F] text-[#fff]
             hover:cursor-pointer hover:bg-[#fff] hover:text-[#00D77F]
             rounded-md font-semibold w-[7rem] h-[4rem]">
             Order now
          </button>

          <button type="submit" class="text-[#000] hover:cursor-pointer 
                hover:text-[#FFF] rounded-md font-semibold w-[7rem] h-[4rem]">
                Explore more
          </button>

      </div>
    </div>

    <div class="z-10 bg-repeat-y bg-[#091B26] w-[46rem]">

    </div>
  </section>
    
  </main>
</template>

<style scoped>
@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
