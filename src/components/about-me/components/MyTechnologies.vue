<template>
    <div class="flex gap-10 px-9 pb-6">
        <TechIconVue />
        <p class="font-bold text-lg">My Tech</p>
    </div>

    <div class="grid grid-cols md:grid-cols-2 lg:grid-cols-3 gap-3 px-9">
        <div v-for="tech in techList" :key="tech" class="card border border-gray-800 py-2 px-2 flex items-center justify-start rounded-lg">
            <p>{{ tech }}</p>
        </div>
 
    </div>
</template>

<script>
import TechIconVue from '@/components/Tech-icon/TechIcon.vue'
export default {
    data() {
        return {
            techList: ['Vue.js', 'Nest.js','Flutter',  'Dart', 'Python', 'Javascript', 'TypeScript', 'Git', 'GitHub', 'MySql', 'Firebase']
        }
    },
    components: {TechIconVue}
}
</script>

<style scoped>

</style>