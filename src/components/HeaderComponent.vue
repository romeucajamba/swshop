<script setup lang="ts">
import { RouterLink, RouterView  } from 'vue-router'
import MenuIcon from 'vue-material-design-icons/Menu.vue';
import MdIconCart from 'vue-material-design-icons/Cart.vue';
import MdIconMagnify from 'vue-material-design-icons/Magnify.vue';

components: {
  MenuIcon;
  MdIconCart;
  MdIconMagnify;
};


</script>

<template>
  <header class="bg-gradient-to-r from-[#FFF8CE] from-50% to-[#091B26] to-10% w-screen h-20 flex flex-row space-x-7">

    
    <div class="w-[15rem] flex flex-row mt-4">
        <img alt="Vue logo" class="w-[3rem] h-[3rem] ml-6" src="@/components/icons/logoSmart.png" width="125" height="125" /> 
        <h1 class="font-semibold text-[2rem] text-[#545C6B]"><span class="text-[#f2a379]">SW</span>Shop</h1>
    
    </div>
    <nav class="w-[25rem] flex flex-row items-center justify-between">
        <RouterLink to="/" class="text-[#545C6B] font-semibold">Home</RouterLink>
        <RouterLink to="/about" class="text-[#545C6B] font-semibold">About</RouterLink>
        <RouterLink to="/product" class="text-[#fff] font-semibold">Product</RouterLink>
        <RouterLink to="/shop" class="text-[#fff] font-semibold">Shop</RouterLink>
    </nav>

    <div class="flex flex-row w-[25rem] h-20 pt-6 pl-14">
        <input type="text" placeholder="pesquise o Smart Watch que queres" class="w-[20rem] h-[2.5rem] border-2 rounded-md pl-1 focus:outline-none z-0 text-[#545C6B] font-semibold">
        <MdIconMagnify class="absolute ml-[21%] mt-2 z-30 text-[#545C6B] hover:cursor-pointer"/>
    </div>

    <MdIconCart class="text-[#fff] hover:cursor-pointer"/>
    
    <button type="button" class="bg-[#00D77F] text-[#fff] hover:cursor-pointer hover:bg-[#fff] hover:text-[#00D77F] rounded-md font-semibold w-[6.5rem] h-[3.5rem]">Get Start</button>
  </header>

  <RouterView />
</template>

<style scoped>

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>