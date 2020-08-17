<template>
  <div class="max-h-full back w-full lg:flex lg:flex-col bg-gray-200">
    <div class="pt-48 px-8 relative w-full bg-gray-200 lg:pt-4">
      <div class="container ml-4">
        <h1 class="text-xl font-semibold text-gray-700">
          Los Angeles
        </h1>
        <p class="text-gray-600">
          Live like the stars in these luxurious Southern California estates.
        </p>
      </div>
      <div class="flex flew-row space-x-5">
        <carousel class="space-x-4 cursor-pointer mx-auto w-full">
          <slide class="mx-4">
            <Review />
          </slide>
          <slide class="mx-4">
            <Review />
          </slide>
          <slide class="mx-4">
            <Review />
          </slide>
          <slide class="mx-4">
            <Review />
          </slide>
          <slide class="mx-4">
            <Review />
          </slide>
        </carousel>
      </div>
    </div>
    <div class="pt-12 lg:mt-0 px-8 relative w-full bg-gray-200">
      <div class="container ml-4">
        <h1 class="text-xl font-semibold text-gray-700">
          Los Angeles
        </h1>
        <p class="text-gray-600">
          Live like the stars in these luxurious Southern California estates.
        </p>
      </div>
      <div class="flex flew-row space-x-5">
        <carousel class="space-x-4 cursor-pointer lg:z-50 mx-auto w-full">
          <slide class="mx-4">
            <Review />
          </slide>
          <slide class="mx-4">
            <Review />
          </slide>
          <slide class="mx-4">
            <Review />
          </slide>
          <slide class="mx-4">
            <Review />
          </slide>
          <slide class="mx-4">
            <Review />
          </slide>
        </carousel>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Review from './Review.vue'

export default Vue.extend({
  components: {
    Review
  }  
})
</script>

<style scoped>
.back {
  z-index: -1200;
}
@media (min-width: 1023px) {
  .back {
    z-index: 50;
  }
}
</style>