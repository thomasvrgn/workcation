<template>
  <div class="p-4">
    <button class="bg-gray-700 text-white font-semibold py-2 px-8 rounded-r-sm focus:outline-none hover:bg-gray-800 focus:bg-gray-900 transition-colors duration-150" @click=open id="sidebarButton">
      Filters
    </button>
    <div class="absolute inset-0 h-full w-2/6 bg-gray-700 transition duration-500 overflow-y-auto" id="sidebar">
      <br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
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
          if (!['sidebarButton', 'sidebar'].includes(e.target.id)) {
            sidebar.style.transform = 'translateX(' + -sidebar.offsetWidth + 'px)'
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