<template class="bg-gray-200">
  <!-- <div class="absolute inset-0 h-full w-full flex flex-row">
    <div class="flex flex-col w-1/5">
      <div class="flex flex-initial bg-blue-400 h-16">
        <Logo />
      </div>
      <div class="flex flex-auto bg-red-400">
        <Sidebar />
      </div>
    </div>
    <div class="flex flex-col w-4/5">
      <div class="flex flex-initial bg-purple-400 h-16">
        <Navbar />
      </div>
      <div class="flex flex-auto bg-green-400">
        <Results />
      </div>
    </div>
  </div> -->
  <div class="bg-gray-200 max-h-full absolute w-full z-10 lg:flex-col lg:flex">
    <div class="fixed w-full lg:flex lg:flex-row lg:relative lg:flex-initial lg:h-20">
      <div class="bg-gray-800 z-40 relative lg:w-1/5 lg:flex lg:fixed">
        <Logo class="lg:flex lg:flex-row" />
      </div>
      <Navbar class="z-30 lg:w-4/5 lg:flex lg:items-center lg:right-0 lg:absolute" />
    </div>
    <div class="lg:flex lg:flex-row lg:flex-auto">
      <Sidebar class="lg:flex lg:w-1/5 lg:fixed" />
      <Results class="h-full lg:max-h-full lg:h-auto absolute bg-gray-200 w-full lg:flex right-0 lg:w-4/5" />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Logo from '@/components/Logo.vue'
import Sidebar from '@/components/Sidebar.vue'
import Navbar from '@/components/Navbar.vue'
import Results from '@/components/Results.vue'

export default Vue.extend({
  components: {
    Logo,
    Sidebar,
    Navbar,
    Results
  }
})
</script>
