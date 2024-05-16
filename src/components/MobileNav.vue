<template>
  <div class="lg:hidden">

    <router-link class="block w-24 mx-auto my-7" to="/">
      <img src="@/assets/zen.png" class="w-24 h-24" @click="closeMenu">
    </router-link>

    <div class="absolute top-0 z-10 w-12 h-12 right-3" @click="toggleMenu">
      <span class="inline-block w-8 h-0.5 absolute rounded-sm top-7 bg-white" :class="menuOpen ? 'hidden' : 'inline-block'"></span>
      <span class="duration-500 inline-block w-8 h-0.5 absolute rounded-sm top-9 bg-white" :class="menuOpen ? '-rotate-45 bg-green-400' : 'rotate-0'"></span>
      <span class="duration-500 inline-block w-8 h-0.5 absolute rounded-sm top-9 bg-white" :class="menuOpen ? 'rotate-45 bg-green-400' : 'rotate-0'"></span>
      <span class="inline-block w-8 h-0.5 absolute rounded-sm top-11 bg-white" :class="menuOpen ? 'hidden' : 'inline-block'"></span>
    </div>

    <div class="absolute top-0 right-0 w-48 overflow-hidden h-96">
      <div class="absolute flex flex-col justify-between w-48 transition duration-500 bg-black border border-white h-96 right-100" :class="menuOpen ? '-translate-x-0' : 'translate-x-full'" >

        <nav class="self-center">
          <ul class="flex flex-col pt-5" @click="closeMenu">
            <li class="my-2 mr-8 text-white cursor-pointer"><router-link to="/">Portfolio</router-link></li>
            <li class="my-2 mr-8 text-white cursor-pointer"><router-link to="/about">About Me</router-link></li>
            <li class="my-2 mr-8 text-white cursor-pointer"><router-link to="/contact">Contact Me</router-link></li>
          </ul>
        </nav>

        <div class="flex flex-col mb-5">
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
    </div>

  </div>
</template>

<script>
export default {
  name: "MobileNav",

  data() {
    return {
      menuOpen: false
    }
  },

  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen
    },
    closeMenu() {
      this.menuOpen = false
    }
  }
}
</script>
