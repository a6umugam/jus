<template>
  <div class="navbar">
      <div class="navbar-content">
          <img src="~/assets/jus-logo.svg" alt="logo" width=64 v-on:click="goto('/')" class="logo">
          <div class="nav-links">
              <a href="/services">Services</a>
              <a href="/portfolio">Portfolio</a>
              <a href="/about">About Us</a>
          </div>
          <div class="nav-buttons">
              <button v-on:click="goto('/contact')">Contact Us</button>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    methods:{
        goto(path){
            this.$router.push(path)
        }
    }
}
</script>

<style>
.logo{
    cursor: pointer;
}
.navbar{
    display: flex;
    width: 100%;
    justify-content: center;
    align-items: center;
    height: 100px;
    padding: 10px;
}

.navbar-content{
    display: flex;
    width: 100vw;
    max-width: 1100px;
    justify-content: space-between;
    align-items: center;
}

.nav-links{
  width: 500px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

@media screen and (max-width: 800px){
    .nav-links{
        display: none;
    }
}

</style>