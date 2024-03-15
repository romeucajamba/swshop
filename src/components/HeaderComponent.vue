<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
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
  <header class="bg-blue-700 w-screen h-20 flex flex-row space-x-[10rem]">

    <div class="bg-[#fff8CE] flex flex-row w-[3rem] h-[3rem]">
        <img alt="Vue logo" class="logo" src="@/components/icons/logoSmart.png" width="125" height="125" />
        <h1>SWShop</h1>
    </div>
    
      <nav class="bg-red-700">
        <RouterLink to="/" class="text-[#000]">Home</RouterLink>
        <RouterLink to="/about" class="text-[#fff]">About</RouterLink>
      </nav>

      <div>
         <MenuIcon/>
         <MdIconCart/>
         <MdIconMagnify/>
        
      </div>
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