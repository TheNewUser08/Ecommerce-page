
<template>
  <nav class="shadow-md w-full fixed top-0 h-12 rounded-b-lg flex items-center">
    <h1 class="font-extrabold text-2xl m-10">
      sneakers
    </h1>
    <div class="flex items-center">
      <div class="m-5 text-center">
        <router-view to="/">
          Collection
        </router-view>
      </div>
      <div class="m-5 hover:cursor-pointer">
        <router-view to="/">
          Men
        </router-view>
      </div>

      <div class="m-5 hover:cursor-pointer">
        <router-view to="/">
          Women
        </router-view>
      </div>

      <div class="m-5 hover:cursor-pointer">
        <router-view to="/">
          About
        </router-view>
      </div>

      <div class="m-5 hover:cursor-pointer">
        <router-view to="/">
          Contact
        </router-view>
      </div>
    </div>
  </nav>
</template>
