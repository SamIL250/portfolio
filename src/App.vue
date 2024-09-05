<template> 
  <div class="main">
    <router-view/>
  </div>

</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:ital,wght@0,200..800;1,200..800&display=swap');

*{
  box-sizing: border-box;
}

#app {
  font-family: "Plus Jakarta Sans";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale; 
  color: #2c3e50;
} 

body
{
  background: black;
}

.main{
  width: 100%;
  min-height: 80vh;
}

/* nav a.router-link-exact-active {
  color: #42b983;
} */
</style>
