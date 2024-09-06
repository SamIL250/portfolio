<template>
    <div class="flex gap-10 px-5 pb-4">
        <TechIconVue />
        <p class="font-bold text-lg">My Tech</p>
    </div>

    <div>
        <marquee behavior="smooth" direction="left">
            <div class="flex gap-5">
            </div>
        </marquee>
    </div>
</template>

<script>
import TechIconVue from '@/components/Tech-icon/TechIcon.vue'
export default {
    components: {TechIconVue}
}
</script>

<style scoped>

</style>