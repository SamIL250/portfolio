<template>
  <div class="grid grid-cols-12">
    <div class="col-span-12 md:col-span-3 min-h-12">
      <!-- profile component here -->
      <ProfileVue />
    </div>
    <div class="col-span-12 md:col-span-4 min-h-12">
      <!-- about me component here -->
      <AboutVue />
    </div>
    <div class="col-span-12  md:col-span-5 min-h-12"> </div>
  </div>
</template>

<script>
// imports
import ProfileVue from '@/components/profile/Profile.vue'
import AboutVue from '@/components/about-me/About.vue'

export default { 
  data() {
    return{}
  },

  components: {
    ProfileVue,
    AboutVue
  }
}
</script>

<style scoped>
  .col-span-12, .col-span-12{
    border-right: 1px solid #3a3a3a;
  } 
</style>  