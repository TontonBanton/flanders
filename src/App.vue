<template>
  <div id="app">
    <MobileNav />
    <div class="justify-between hidden w-10/12 h-16 mx-auto my-10 lg:flex">

      <nav class="self-center w-5/12">
        <ul class="flex">
          <li class="mr-8 text-lg text-white cursor-pointer"><router-link to="/">Portfolio</router-link></li>
          <li class="mr-8 text-lg text-white cursor-pointer"><router-link to="/about">About Me</router-link></li>
          <li class="mr-8 text-lg text-white cursor-pointer"><router-link to="/contact">Contact Me</router-link></li>
        </ul>
      </nav>

      <router-link to="/">
        <img src="@/assets/zen.png" class="self-center w-24 h-24">
      </router-link>


      <div class="flex justify-end w-5/12 h-16">
        <a href="https://www.instagram.com/the_shred_flanders/" target="_blank" class="my-auto cursor-pointer ml-7">
          <i class="text-2xl text-white fa-brands fa-instagram"></i>
        </a>
        <a href="https://www.facebook.com/profile.php?id=100083959629324" target="_blank" class="my-auto cursor-pointer ml-7">
          <i class="text-2xl text-white fa-brands fa-facebook"></i>
        </a>
        <a href="https://www.linkedin.com/in/shred-flanders-356896246/" target="_blank" class="my-auto cursor-pointer ml-7">
          <i class="text-2xl text-white fa-brands fa-linkedin"></i>
        </a>
        <a href="https://twitter.com/ShredFlanders4" target="_blank" class="my-auto cursor-pointer ml-7">
          <i class="text-2xl text-white fa-brands fa-twitter"></i>
        </a>

      </div>
    </div>
    <router-view/>
  </div>
</template>

<script>
import MobileNav from './components/MobileNav.vue';

export default {
  name: "App",
  components: { MobileNav }

}
</script>


