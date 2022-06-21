<template>
  <div class="navbar">

      <div class="navbar-content">
          <img src="~/assets/jus_metal.svg" alt="logo" width=350 heigh v-on:click="goto('/')" class="logo">
          <div class="nav-links">
              <a href="/services">What we Offer</a>
              <a href="/portfolio">Portfolio</a>
              <a href="/about">About Us</a>
              <a href="/contact">Contact Us</a>
          </div>
          <div class="nav-buttons">
              <button v-on:click="formView = !formView" >Get Free Quotation</button>
          </div>
      </div>
      <div class="mobile-bar">
        <a href="/services">Services</a>
        <a href="/portfolio">Portfolio</a>
        <a href="/about">About Us</a>
      </div>

      <div class="info-bar">
        <div>
            <section>
            <p>Call Us : 514.292.3162</p>
            <p>Email : contact@jus.ca</p>
            </section>
            <p>We pride ourselves on guiding our clients to success - and creating intelligent solutions that minimize risks and maximize rewards. </p>
            <!-- <a href="#">Work with us</a>
            <a href="#">Web Design</a>
            <a href="#">Mobile App Development</a> -->
        </div>
      </div>

    <ContactForm v-if="formView" @closeMenu="formView = !formView" />

  </div>
</template>

<script>
export default {
    data() {
    return {
        formView:false
    };
  },

    methods:{
        goto(path){
            this.$router.push(path)
        }
    },
}
</script>

<style>
.info-bar{
    background-color: #48ff87;
    width: 100%;
    justify-content: space-evenly;
    height: 80px;
    align-items: center;
    display: flex;
}

.info-bar section{
    width: 400px;
}
.info-bar div{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    max-width: 1100px;
}
.info-bar p{
    color: #435264;
    font-size: large;
}

.info-bar h2{
    color: #181818;
}

.mobile-bar{
    background-color: #0f171f;
    width: 100%;
    justify-content: space-evenly;
    height: 40px;
    align-items: center;
    display: none;
}

.logo{
    cursor: pointer;
}
.navbar{
    display: flex;
    flex-flow: column;
    width: 100%;
    justify-content: center;
    align-items: center;
    /* height: 100px; */
}

.navbar-content{
    padding: 10px;
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

    .mobile-bar{
        display: flex;
        margin-bottom: 20px;
    }

    .info-bar{
        display: none;
    }
}

</style>