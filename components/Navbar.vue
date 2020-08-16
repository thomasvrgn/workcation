<template>
  <nav class="bg-white pt-4" :class="{'py-4': !opened}">
    <div class="container flex flex-row flex-wrap mx-auto">
      <div class="flex flex-auto w-1/2 items-center">
        <div class="container flex-row flex">
          <span class="flex items-center mr-6 cursor-pointer text-gray-800" @click=openNavbar>
                <button class="menu focus:outline-none text-gray-800" :class="{'opened': opened}" aria-label="Main Menu">
                  <svg width="32" height="32" viewBox="0 0 100 100">
                    <path class="line line1" d="M 20,29.000046 H 80.000231 C 80.000231,29.000046 94.498839,28.817352 94.532987,66.711331 94.543142,77.980673 90.966081,81.670246 85.259173,81.668997 79.552261,81.667751 75.000211,74.999942 75.000211,74.999942 L 25.000021,25.000058" />
                    <path class="line line2" d="M 20,50 H 80" />
                    <path class="line line3" d="M 20,70.999954 H 80.000231 C 80.000231,70.999954 94.498839,71.182648 94.532987,33.288669 94.543142,22.019327 90.966081,18.329754 85.259173,18.331003 79.552261,18.332249 75.000211,25.000058 75.000211,25.000058 L 25.000021,74.999942" />
                  </svg>
                </button>
          </span>
          <span class="bg-gray-100 flex items-center text-gray-500 w-10/12 rounded-md">
            <svg width="20" height="20" class="mx-2" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M18.319 14.4326C20.7628 11.2941 20.542 6.75347 17.6569 3.86829C14.5327 0.744098 9.46734 0.744098 6.34315 3.86829C3.21895 6.99249 3.21895 12.0578 6.34315 15.182C9.22833 18.0672 13.769 18.2879 16.9075 15.8442C16.921 15.8595 16.9351 15.8745 16.9497 15.8891L21.1924 20.1317C21.5829 20.5223 22.2161 20.5223 22.6066 20.1317C22.9971 19.7412 22.9971 19.1081 22.6066 18.7175L18.364 14.4749C18.3493 14.4603 18.3343 14.4462 18.319 14.4326ZM16.2426 5.28251C18.5858 7.62565 18.5858 11.4246 16.2426 13.7678C13.8995 16.1109 10.1005 16.1109 7.75736 13.7678C5.41421 11.4246 5.41421 7.62565 7.75736 5.28251C10.1005 2.93936 13.8995 2.93936 16.2426 5.28251Z" fill="currentColor" /></svg>
            <input type="text" class="bg-transparent py-1 my-1 text-gray-500 placeholder-gray-500 focus:outline-none" name="" id="" placeholder="Search by keywords">
          </span>
        </div>
      </div>
      <div class="flex flex-auto flex-col space-y-2 order-last list-none my-5 font-medium text-gray-800" :class="{'hidden': !opened}">
        <li class="cursor-pointer hover:text-gray-900 hover:bg-gray-100 px-4 py-2 rounded-md">
          List your property
        </li>
        <li class="cursor-pointer hover:text-gray-900 hover:bg-gray-100 px-4 py-2 rounded-md">
          Trips
        </li>
        <li class="cursor-pointer hover:text-gray-900 hover:bg-gray-100 px-4 py-2 rounded-md">
          Messages
        </li>
        <li class="cursor-pointer hover:text-gray-900 hover:bg-gray-100 px-4 py-2 rounded-md">
          Support
        </li>
      </div>
      <div class="flex flex-auto w-1/2 justify-end">
        <img src="https://th.bing.com/th/id/OIP.Zb5-XDMwL991BL0cXnqj-gHaHa?pid=Api&rs=1" class="w-12 h-12 rounded-full" alt="">
      </div>
    </div>
  </nav>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data: () => ({
    opened: false
  }),
  methods: {
    openNavbar: function () : void {
      this.opened = !this.opened
    }
  }
})
</script>

<style>
.menu {
  background-color: transparent;
  border: none;
  cursor: pointer;
  display: flex;
  padding: 0;
}
.line {
  fill: none;
  stroke: #2d3748;
  stroke-width: 6;
  transition: stroke-dasharray 600ms cubic-bezier(0.4, 0, 0.2, 1),
    stroke-dashoffset 600ms cubic-bezier(0.4, 0, 0.2, 1);
}
.line1 {
  stroke-dasharray: 60 207;
  stroke-width: 6;
}
.line2 {
  stroke-dasharray: 60 60;
  stroke-width: 6;
}
.line3 {
  stroke-dasharray: 60 207;
  stroke-width: 6;
}
.opened .line1 {
  stroke-dasharray: 90 207;
  stroke-dashoffset: -134;
  stroke-width: 6;
}
.opened .line2 {
  stroke-dasharray: 1 60;
  stroke-dashoffset: -30;
  stroke-width: 6;
}
.opened .line3 {
  stroke-dasharray: 90 207;
  stroke-dashoffset: -134;
  stroke-width: 6;
}
</style>