<template>
  <nav class="bg-white pt-4">
    <div class="container flex flex-row flex-wrap mx-auto">
      <div class="flex flex-auto w-1/2 items-center">
        <div class="container flex-row flex">
          <span class="flex items-center mr-6 cursor-pointer text-gray-800">
            <svg width="32" height="32" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M2 6C2 5.44772 2.44772 5 3 5H21C21.5523 5 22 5.44772 22 6C22 6.55228 21.5523 7 21 7H3C2.44772 7 2 6.55228 2 6Z" fill="currentColor" /><path d="M2 12.0322C2 11.4799 2.44772 11.0322 3 11.0322H21C21.5523 11.0322 22 11.4799 22 12.0322C22 12.5845 21.5523 13.0322 21 13.0322H3C2.44772 13.0322 2 12.5845 2 12.0322Z" fill="currentColor" /><path d="M3 17.0645C2.44772 17.0645 2 17.5122 2 18.0645C2 18.6167 2.44772 19.0645 3 19.0645H21C21.5523 19.0645 22 18.6167 22 18.0645C22 17.5122 21.5523 17.0645 21 17.0645H3Z" fill="currentColor" /></svg>
          </span>
          <span class="bg-gray-100 flex items-center text-gray-500 w-10/12 rounded-md">
            <svg width="20" height="20" class="mx-2" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M18.319 14.4326C20.7628 11.2941 20.542 6.75347 17.6569 3.86829C14.5327 0.744098 9.46734 0.744098 6.34315 3.86829C3.21895 6.99249 3.21895 12.0578 6.34315 15.182C9.22833 18.0672 13.769 18.2879 16.9075 15.8442C16.921 15.8595 16.9351 15.8745 16.9497 15.8891L21.1924 20.1317C21.5829 20.5223 22.2161 20.5223 22.6066 20.1317C22.9971 19.7412 22.9971 19.1081 22.6066 18.7175L18.364 14.4749C18.3493 14.4603 18.3343 14.4462 18.319 14.4326ZM16.2426 5.28251C18.5858 7.62565 18.5858 11.4246 16.2426 13.7678C13.8995 16.1109 10.1005 16.1109 7.75736 13.7678C5.41421 11.4246 5.41421 7.62565 7.75736 5.28251C10.1005 2.93936 13.8995 2.93936 16.2426 5.28251Z" fill="currentColor" /></svg>
            <input type="text" class="bg-transparent py-1 my-1 text-gray-500 placeholder-gray-500 focus:outline-none" name="" id="" placeholder="Search by keywords">
          </span>
        </div>
      </div>
      <div class="flex flex-auto flex-col space-y-2 order-last list-none my-5 font-medium text-gray-800">
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