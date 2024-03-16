<script setup lang="ts">

defineProps<{
  msg: string
}>()

</script>

<template>
  <main>
   
  <section class="flex flex-row bg-[#fff] w-screen h-[50rem]">
    <div class="absolute z-20 flex flex-col space-y-6 p-4 w-[20rem] h-[8rem] bg-[#FFCFCF] rounded-[0.5rem] border-solid">
        <h3 class="text-[#373645] font-semibold">{{ msg }}</h3>
        <p class="text-[#B79AA1]">You can get up to 10 percent discount from here!</p>
    </div>

    <div class="bg-[#FFF8CE] z-10">

      <h2>Explore our new colections</h2>

      <p>Every man needs a good solid watch. I onw many
         watches, but this on is <br/>usually the one my wrist.
         It's help you track you all day steps, colories <br/> 
        consumptions, distance traveled & heart rate.
      </p>
      <div>
          <button type="submit">Order now</button>
          <button type="submit">Explore more</button>
      </div>
    </div>
    <div class="z-10 bg-gradient-to-r from-[#091B26] "></div>
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
