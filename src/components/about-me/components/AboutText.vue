<template>
  <div class="grid gap-5 px-5 py-4">
    <p class="text-justify text-">
        Since the beginning, I've been deeply passionate about computer science, 
        starting with no-code tools back in 2021. This early fascination led me to
        teach myself how to code, and over the years, I've honed my skills across
        various programming languages and technologies.
    </p>
    <p class="text-justify text-">
        I've had the privilege of working in a web development company, and now, I'm 
        eager to build innovative projects, automate tasks, and push the boundaries 
        in Web & Mobile Development, Open Source, and Competitive Programming.
    </p>

    <div class="mb-16">
      <p>As a developer, I specialize in designing and building responsive software that
         seamlessly adapts to any screen size. Whether it's a mobile phone, tablet, or 
         desktop, I ensure that each interface is fluid and user-friendly.</p>
    </div>
    <div class="relative mb-24 ">
      <ScreensVue />
    </div>
  </div>
</template>

<script>
import ScreensVue from '@/components/devices-screens/Screens.vue'
export default {
  components: {ScreensVue}
}
</script>

<style>

</style>