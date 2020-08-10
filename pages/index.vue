<template>
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
  <div class="bg-gray-200 min-h-full max-h-screen absolute w-full z-10">
    <div class="bg-gray-800 z-50 relative">
      <Logo />
    </div>
    <Navbar class="z-50" />
    <Sidebar />
    <Results class="max-h-full absolute" />
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
