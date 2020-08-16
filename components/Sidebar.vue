<template>
  <div class="p-4">
    <button class="bg-gray-700 text-white font-semibold py-2 px-8 rounded-r-sm focus:outline-none hover:bg-gray-800 focus:bg-gray-900 transition-colors duration-150 absolute back" @click=open id="sidebarButton">
      Filters
    </button>
    <div class="absolute inset-0 h-full w-2/6 bg-gray-700 transition duration-500 overflow-y-auto z-50" id="sidebar">
      <form action="">
        <div class="container flex flex-row flex-wrap p-4">
          <div class="flex flex-auto w-3/6 flex-col px-2">
            <label for="" class="block font-semibold text-gray-400 text-sm">
              Bedrooms
            </label>
            <div class="inline-block relative mt-2 cursor-pointer">
              <select class="block appearance-none w-full bg-gray-600   px-4 py-2 pr-8 rounded leading-tight focus:outline-none text-gray-200 cursor-pointer">
                <option>1</option>
                <option>2</option>
                <option>3</option>
                <option>4</option>
              </select>
              <div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-white">
                <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
              </div>
            </div>
          </div>
          <div class="flex flex-auto w-3/6 flex-col px-2">
            <label for="" class="block font-semibold text-gray-400 text-sm">
              Bathrooms
            </label>
            <div class="inline-block relative mt-2 cursor-pointer">
              <select class="block appearance-none w-full bg-gray-600   px-4 py-2 pr-8 rounded leading-tight focus:outline-none text-gray-200 cursor-pointer">
                <option>1</option>
                <option>2</option>
                <option>3</option>
                <option>4</option>
              </select>
              <div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-white">
                <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
              </div>
            </div>
          </div>
          <div class="flex flex-auto flex-col px-2 mt-4">
            <label for="" class="block font-semibold text-gray-400 text-sm">
             Price Range
            </label>
            <div class="inline-block relative mt-2 cursor-pointer">
              <select class="block appearance-none w-full bg-gray-600   px-4 py-2 pr-8 rounded leading-tight focus:outline-none text-gray-200 cursor-pointer">
                <option>Up to $2,000 /wk</option>
              </select>
              <div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-white">
                <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
              </div>
            </div>
          </div>
        </div>
        <hr class="border-gray-800 border">
        <div class="container flex flex-col p-4">
          <label for="" class="block font-semibold text-gray-400 text-sm mb-3">
            Property type
          </label>
          <li class="flex flex-row">
            <span class="flex flex-initial relative items-center mr-2 cursor-pointer">
              <span class="relative flex items-center h-5 w-5 bg-indigo-500 rounded-full flex-row">
                <span class="relative flex justify-center items-center h-2 w-2 bg-white mx-auto rounded-full"></span>
              </span>
            </span>
            <span class="flex flex-auto text-white">
              House
            </span>
          </li>
          <li class="flex flex-row mt-3">
            <span class="flex flex-initial relative items-center mr-2 cursor-pointer">
              <span class="relative flex items-center h-5 w-5 bg-gray-800 rounded-full flex-row">
              </span>
            </span>
            <span class="flex flex-auto text-white">
              Apartment
            </span>
          </li>
          <li class="flex flex-row mt-3">
            <span class="flex flex-initial relative items-center mr-2 cursor-pointer">
              <span class="relative flex items-center h-5 w-5 bg-gray-800 rounded-full flex-row">
              </span>
            </span>
            <span class="flex flex-auto text-white">
              Loft
            </span>
          </li>
          <li class="flex flex-row mt-3">
            <span class="flex flex-initial relative items-center mr-2 cursor-pointer">
              <span class="relative flex items-center h-5 w-5 bg-gray-800 rounded-full flex-row">
              </span>
            </span>
            <span class="flex flex-auto text-white">
              Townhouse
            </span>
          </li>
        </div>
        <hr class="border-gray-800 border">
        <div class="container flex flex-col p-4 mb-20">
          <label for="" class="block font-semibold text-gray-400 text-sm mb-3">
            Amenities
          </label>
          <li class="flex flex-row mt-3">
            <span class="flex flex-initial relative items-center mr-2 cursor-pointer">
              <span class="relative flex items-center h-5 w-5 bg-gray-800 rounded flex-row">
              </span>
            </span>
            <span class="flex flex-auto text-white">
              Balcony
            </span>
          </li>
          <li class="flex flex-row mt-3">
            <span class="flex flex-initial relative items-center mr-2 cursor-pointer">
              <span class="relative flex items-center h-5 w-5 bg-gray-800 rounded flex-row">
              </span>
            </span>
            <span class="flex flex-auto text-white">
              Air conditioning
            </span>
          </li>
          <li class="flex flex-row mt-3">
            <span class="flex flex-initial relative items-center mr-2 cursor-pointer">
              <span class="relative flex items-center h-5 w-5 bg-indigo-500 rounded flex-row">
                <svg width="32" class="text-white" height="32" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M10.5858 13.4142L7.75735 10.5858L6.34314 12L10.5858 16.2427L17.6568 9.1716L16.2426 7.75739L10.5858 13.4142Z" fill="currentColor" /></svg>
              </span>
            </span>
            <span class="flex flex-auto text-white">
              Pool
            </span>
          </li>
          <li class="flex flex-row mt-3">
            <span class="flex flex-initial relative items-center mr-2 cursor-pointer">
              <span class="relative flex items-center h-5 w-5 bg-gray-800 rounded flex-row">
              </span>
            </span>
            <span class="flex flex-auto text-white">
              Beach
            </span>
          </li>
          <li class="flex flex-row mt-3">
            <span class="flex flex-initial relative items-center mr-2 cursor-pointer">
              <span class="relative flex items-center h-5 w-5 bg-gray-800 rounded flex-row">
              </span>
            </span>
            <span class="flex flex-auto text-white">
              Pet friendly
            </span>
          </li>
          <li class="flex flex-row mt-3">
            <span class="flex flex-initial relative items-center mr-2 cursor-pointer">
              <span class="relative flex items-center h-5 w-5 bg-gray-800 rounded flex-row">
              </span>
            </span>
            <span class="flex flex-auto text-white">
              Kid friendly
            </span>
          </li>
          <li class="flex flex-row mt-3">
            <span class="flex flex-initial relative items-center mr-2 cursor-pointer">
              <span class="relative flex items-center h-5 w-5 bg-gray-800 rounded flex-row">
              </span>
            </span>
            <span class="flex flex-auto text-white">
              Parking
            </span>
          </li>
        </div>
        <div class="sticky bottom-0 w-full bg-gray-900 px-4 py-4">
          <button class="bg-indigo-500 w-full block py-2 px-2 font-semibold text-white rounded-md hover:bg-indigo-600 focus:bg-indigo-700 focus:outline-none transition-colors duration-150">
            Update results
          </button>
        </div>
      </form>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
function hasParentWithMatchingSelector (target: EventTarget, selector: string) : any {
  return [...document.querySelectorAll(selector)].some(el =>
    el !== target && el.contains(target)
  )
}
export default Vue.extend({
  data: () => ({
    opened: false
  }),
  mounted: function () {
    const sidebar = document.getElementById('sidebar')
    if (sidebar !== null) {
      sidebar.style.transform = 'translateX(' + -sidebar.offsetWidth + 'px)'
      window.addEventListener('click', function (e) {
        if (e.target !== null) {
          if (!hasParentWithMatchingSelector(e.target, '#sidebar')) {
            if (!['sidebarButton', 'sidebar'].includes(e.target.id)) {
              sidebar.style.transform = 'translateX(' + -sidebar.offsetWidth + 'px)'
            }
          }
        }
      })
    }
  },
  methods: {
    open: function () {
      const sidebar = document.getElementById('sidebar')
      if (sidebar !== null) {
        sidebar.style.transform = 'translateX(0)'
      }
    }
  }
})
</script>

<style>
.back {
  z-index: -1000;
}
#sidebar::-webkit-scrollbar {
  width: 10px;
}

#sidebar::-webkit-scrollbar-track {
  background: #4a5568;
}

#sidebar::-webkit-scrollbar-thumb {
  background: #1a202c;
}

#sidebar::-webkit-scrollbar-thumb:hover {
  background: #555;
}
</style>