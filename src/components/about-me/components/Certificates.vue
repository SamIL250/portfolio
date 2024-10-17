<template>
  <div class="px-9 py-10 pt-20 flex justify-start items-center gap-10">
    <div class="">
      <ProgressVue />
    </div>
    <p class="font-bold text-lg">Certificates</p>
  </div>

  <div class="grid grid-cols md:grid-cols-2 px-20 md:px-9 gap-3">
    <div class="border border-gray-800 rounded-lg p-5 shadow cursor-pointer hover:bg-gray-900 transition">
      <img src="../../../assets/sert.png" alt="" srcset="">
    </div>
    <!-- <div class="border border-gray-800 rounded-lg p-5 shadow cursor-pointer hover:bg-gray-900 transition">
      <img src="../../../assets/sert.png" alt="" srcset="">
    </div>
    <div class="border border-gray-800 rounded-lg p-5 shadow cursor-pointer hover:bg-gray-900 transition">
      <img src="../../../assets/sert.png" alt="" srcset="">
    </div> -->
  </div>
</template>

<script>
import ProgressVue from '@/components/progress_element/Progress.vue'
export default {
  components: {
    ProgressVue
  }
}
</script>

<style scoped>

</style>