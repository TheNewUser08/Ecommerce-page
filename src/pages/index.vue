<template>
  <div class="flex justify-between m-auto w-3/7 mt-40">
    <div>
      <div class="mb-3">
        <img :src="image" alt="" class="min-w-60 rounded-lg w-90">
      </div>
      <div class="flex w-90 min-w-60 justify-between">
        <img src="public\images\image-product-1-thumbnail.jpg" alt="sneaker image" class="w-17 rounded-lg cursor-pointer" @click="choseImage('public/images/image-product-1-thumbnail.jpg')">
        <img src="public\images\image-product-2-thumbnail.jpg" alt="sneaker image" class="w-17 rounded-lg cursor-pointer" @click="choseImage('public/images/image-product-2-thumbnail.jpg')">
        <img src="public\images\image-product-3-thumbnail.jpg" alt="sneaker image" class="w-17 rounded-lg cursor-pointer" @click="choseImage('public/images/image-product-3-thumbnail.jpg')">
        <img src="public\images\image-product-4-thumbnail.jpg" alt="sneaker image" class="w-17 rounded-lg cursor-pointer" @click="choseImage('public/images/image-product-4-thumbnail.jpg')">
      </div>
    </div>
    <div class=" text-left w-2/5 ml-12">
      <h3 class="font-semibold text-sm mb-4 orange">
        Sneaker Company
      </h3> <h2 class="text-3xl font-black max-w-70">
        Fall Limited Edition Sneakers
      </h2>
      <p class="mt-9 font-normal">
        These low-profile sneakers are your perfect casual wear companion. Featuring a
        durable rubber outer sole, they’ll withstand everything the weather can offer.
      </p>
      <div class="mt-3">
        <p class="font-bold text-xl inline ">
          $125.00
        </p>
        <p class="bg-orange-200 orange w-min inline font-semibold p-1 ml-2 text-sm">
          50%
        </p>
        <p class="text-gray-400 line-through text-sm">
          $250.00
        </p>
      </div>
      <div>
        <button class="bg-orange-400 text-white px-8 py-2 rounded-lg shadow-gray-400 shadow-md">
          <div class="inline">
            Add to cart
          </div>
          <img src="public\images\icon-cart.svg" alt="shoping cart icon" fill="white" class="inline">
        </button>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
const image = ref('public/images/image-product-1-thumbnail.jpg')

const choseImage = (img: string) => {
  image.value = img
}
</script>
