<template>
    <div class="flex px-6 py-5 pt-10 md:py-4 gap-5 items-center font-bold text-lg shadow"> 
        <AboutMeAnimeVue />
        <p>About me</p>
    </div>
</template>

<script>
import AboutMeAnimeVue from '../../about-me-icon/AboutMeAnime.vue'
export default {
    data() {
        return {
            // Add your data here
        }
    },

    components: {
        AboutMeAnimeVue
    }
}
</script>

<style scoped>

</style>