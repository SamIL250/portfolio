<template>
    <NavbarVue />
    <AboutTextVue />
    <MyTechnologiesVue />
    <CertificatesVue />
</template>

<script>
import AboutMeAnimeVue from '../about-me-icon/AboutMeAnime.vue'
import NavbarVue from './components/Navbar.vue'
import AboutTextVue from './components/AboutText.vue'
import MyTechnologiesVue from './components/MyTechnologies.vue'
import CertificatesVue from './components/Certificates.vue'
export default {
    data() {
        return {
            // Add your data here
        }
    },

    components: {
        AboutMeAnimeVue,
        NavbarVue,
        AboutTextVue,
        MyTechnologiesVue,
        CertificatesVue,
    }
}
</script>

<style scoped>

</style>