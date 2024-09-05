<template>
  <div class="grid grid-cols-12">
    <div class="col-span-3 min-h-12 border-r">
      <!-- profile component here -->
      <ProfileVue />
    </div>
    <div class="col-span-4 min-h-12 border-r"></div>
    <div class="col-span-5 min-h-12 border-l"></div>
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

<style>

</style>