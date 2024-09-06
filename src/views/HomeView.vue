<template>
  <div class="grid grid-cols-12">
    <div class="col-span-3 min-h-12">
      <!-- profile component here -->
      <ProfileVue />
    </div>
    <div class="col-span-4 min-h-12"> </div>
    <div class="col-span-5 min-h-12"> </div>
  </div>
</template>

<script>
// imports
import ProfileVue from '@/components/profile/Profile.vue'

export default { 
  data() {
    return{}
  },

  components: {
    ProfileVue
  }
}
</script>

<style scoped>
  .col-span-3, .col-span-4{
    border-right: 1px solid #3a3a3a;
  } 
</style>  