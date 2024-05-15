<template>
  <div id="app">
    <div class="border border-white justify-between hidden w-10/12 h-16 mx-auto my-10 lg:flex">
      <nav class="self-center w-5/12">
        <ul class="flex">
          <li class="mr-8 text-lg text-white cursor-pointer"><router-link to="/">Portfolio</router-link></li>
          <li class="mr-8 text-lg text-white cursor-pointer"><router-link to="/about">About Me</router-link></li>
          <li class="mr-8 text-lg text-white cursor-pointer"><router-link to="/contact">Contact Me</router-link></li>
        </ul>
      </nav>
    </div>
    <router-view/>
  </div>
</template>


