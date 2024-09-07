<template>
  <div class="loader"></div>
</template>

<script>
export default {

}
</script>

<style scoped> 
.loader {
  width: 37.8px;
  height: 37.8px;
  position: relative;
  transform: rotate(45deg);
}

.loader:before,
.loader:after {
  content: "";
  position: absolute;
  inset: 0;
  border-radius: 50% 50% 0 50%;
  background: #0000;
  background-image: radial-gradient(circle 11.2px at 50% 50%,#0000 94%, #6c6c6c);
}

.loader:after {
  animation: pulse-ytk0dhmd 1s infinite;
  transform: perspective(336px) translateZ(0px);
}

@keyframes pulse-ytk0dhmd {
  to {
    transform: perspective(336px) translateZ(168px);
    opacity: 0;
  }
}
  

</style>