<template>
    <div class="main px-9 py-5">
        <a href="mailto:scamil350@gmail.com">
            <div class="text-center border-2 border-gray-700 py-2 rounded-xl cursor-pointer text-sm md:text">
                <p>Open for Work: Full time / Remote</p>
            </div>
        </a>
        <div class="flex items-center justify-center">
            <div class="my-3">
                <LocationPinVue />
            </div>  
        </div>
        <div class="my-4">
            <WorkTextVue />
        </div>
    </div>
</template>

<script>
import LocationPinVue from './LocationPin.vue'
import WorkTextVue from './WorkText.vue'
export default {
    components: {
        LocationPinVue,
        WorkTextVue
    }
}
</script>

<style scoped>
    .main{
        min-height: 300px;
        background-image: url(../../../assets/globe.svg);
        background-position: center;
        background-size: cover;
    }
</style>