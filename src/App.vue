<template>
  <div id="app">
    <div id="nav">
      <p class="text">HELLO</p>
      <router-link to="/">Home</router-link> |
      <router-link to="/login">Login</router-link> |
       <router-link to="/register">Register</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
export default {}
  document.addEventListener('DOMContentLoaded',()=>{
    const html = document.querySelector('html')
    let fontSize = window.innerWidth / 10
    fontSize = fontSize > 50 ? 50 :fontSize
    html.style.fontSize = fontSize + 'px'
  })
</script>


<style scoped lang="scss">
@import "./assets/styles/global.scss";
  .text {
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: px2rem(20);
    color:blue;

  }
</style>
