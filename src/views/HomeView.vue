<template>
  <div class="grid grid-cols-12 pb-20">
    <div class="col-span-12 md:col-span-3 min-h-12">
      <!-- profile component here -->
      <ProfileVue />
    </div>
    <div class="col-span-12 md:col-span-4 min-h-12">
      <!-- about me component here -->
      <AboutVue />
    </div>
    <div class="col-span-12  md:col-span-5 min-h-12">
      <!-- my works component here -->
      <WorksVue />
    </div>
  </div>
</template>

<script>
// imports
import ProfileVue from '@/components/profile/Profile.vue'
import AboutVue from '@/components/about-me/About.vue'
import WorksVue from '@/components/my-works/Works.vue'

export default { 
  data() {
    return{}
  },

  components: {
    ProfileVue,
    AboutVue,
    WorksVue,
  }
}
</script>

<style scoped>
  .col-span-12, .col-span-12{
    border-right: 1px solid #3a3a3a;
  } 
</style>  