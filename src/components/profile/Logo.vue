<template>
  <div class="flex gap-10 px-10 py-2 shadow items-center">
    <p class="logo">SN</p>
    <a href="">{{ work }}</a>
  </div>
</template>

<script>

export default {
    props: [
        'logo',
        'work'
    ]
}
</script>

<style scoped>
    .logo{
        font-size: 30px;
        font-weight: 800;
    }
</style>