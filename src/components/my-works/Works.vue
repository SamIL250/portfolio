<template>
  <div class="px-9 shadow flex gap-10 pt-16 md:pt-0">
    <LaptopVue />
    <p class="text-lg font-bold py-4">My Works</p>
  </div>

  <div class="">
    <ProjectsVue />
  </div>
  <div class="my-10">
    <OpenForWorkVue />
  </div>
</template>

<script>
import OpenForWorkVue from './components/OpenForWork.vue'
import ProjectsVue from './components/Projects.vue'
import LaptopVue from './components/WorkIcon.vue'
export default {
    components: {
        LaptopVue,
        ProjectsVue,
        OpenForWorkVue
    }
}
</script>

<style scoped>

</style>