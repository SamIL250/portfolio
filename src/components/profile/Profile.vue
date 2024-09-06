<template>
  <div>
    <LogoVue logo="huey2" work="Work" />
    <div class="flex justify-center my-6">
        <div class="border p-5 flex justify-center overflow-hidden bg-black">
            <img src="../../assets/huey2.png" alt="" width="170px" srcset="">
        </div>
    </div>
    <MyDescriptionVue />
  </div>
</template>

<script>
// imports
import LogoVue from '@/components/profile/Logo.vue';
import MyDescriptionVue from './My-Description.vue';
export default {
    data() {
        return {
            // data properties
        }
    },

    components: {
        LogoVue,
        MyDescriptionVue
    }
}
</script>

<style scoped>
    .border{
        border: 1px solid #333;
        border-radius: 50%;
    }
</style>