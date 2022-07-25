<template>
<!-- FRENCH VERSION HERE -->
  <div class="navbar-alt" v-if="isFr">

        <div class="info-bar-alt" v-bind:class="{ incpadding: stickIt }">
        <div>
            <p><img src="~/assets/icons/phone.svg" width="28" alt="people"> <strong>+1 (514) 292-3162</strong> </p>
            <p><img src="~/assets/icons/email.svg" width="28" alt="people"> <strong>info@jusmulticreation.ca</strong> </p>
        </div>
      </div>

      <div class="transbg backdrop-blur small-nav" v-bind:class="{ sticky: stickIt }">
        <div class="navbar-content-alt">
          <img src="~/assets/jus_green_fr.svg" alt="logo" width=350 heigh v-on:click="goto('/')" class="logo">
          <div class="nav-links">
              <a href="/services">Nos Services</a>
              <!-- <a href="/portfolio">Portfolio</a> -->
              <a href="/about">À propos</a>
              <a href="/contact">Contact</a>
          </div>
          <div class="nav-buttons">
              <button v-on:click="goto('/contact')" >Devis gratuit</button>
              <a href="/indexen"><strong>Fr</strong> / En</a>
          </div>
      </div>
      </div>

      <div class="mobile-bar">
        <a href="/services">Nos Services</a>
        <a href="/portfolio">Portfolio</a>
        <a href="/about">À propos</a>
      </div>
  </div>
<!-- ENGLISH VERSION HERE -->
  <div class="navbar-alt" v-else>

        <div class="info-bar-alt" v-bind:class="{ incpadding: stickIt }">
        <div>
            <p><img src="~/assets/icons/phone.svg" width="28" alt="people"> <strong>+1 (514) 292-3162</strong> </p>
            <p><img src="~/assets/icons/email.svg" width="28" alt="people"> <strong>info@jusmulticreation.ca</strong> </p>
        </div>
      </div>

      <div class="transbg backdrop-blur small-nav" v-bind:class="{ sticky: stickIt }">
        <div class="navbar-content-alt">
          <img src="~/assets/jus_green.svg" alt="logo" width=350 heigh v-on:click="goto('/indexen')" class="logo">
          <div class="nav-links">
              <a href="/servicesen">What we Offer</a>
              <!-- <a href="/portfolio">Portfolio</a> -->
              <a href="/abouten">About</a>
              <a href="/contacten">Contact</a>
          </div>
          <div class="nav-buttons">
              <button v-on:click="goto('/contacten')" >Free Quote</button>
              <a href="/">Fr / <strong>En</strong> </a>
          </div>
      </div>
      </div>

      <div class="mobile-bar">
        <a href="/services">Services</a>
        <a href="/portfolio">Portfolio</a>
        <a href="/about">About</a>
      </div>
  </div>
</template>

<script>
export default {
    props:{isFr:false},
    data() {
    return {
        formView:false,
        scrollVal: 0,
        stickIt:false
    };
  },

  beforeMount() {
    window.addEventListener('scroll', this.handleScroll)
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.handleScroll)
  },

    methods:{
        goto(path){
            this.$router.push(path)
        },
        handleScroll() {
            // console.log(window.scrollY)
            this.scrollVal = window.scrollY
            var scrolled = window.scrollY
            if(scrolled >= 50){
                this.stickIt = true
            }else{
                this.stickIt = false
            }
        },
    },
}
</script>

<style>
.nav-buttons{
    display: flex;
    justify-content: center;
    align-items: center;
}

.nav-buttons a{
    margin-left: 10px;
    border: 1.5px solid #12AAF3;
    border-radius: 5px;
    padding: 5px;
}

.nav-buttons a strong{
    color: #e84279;
}
.info-bar-alt{
    /* background-color: #48ff87; */
    background: rgb(0,239,255);
    background: linear-gradient(90deg, rgba(0,239,255,1) 0%, rgba(72,255,128,1) 100%);
    width: 100%;
    justify-content: space-evenly;
    align-items: center;
    padding: 5px;
    display: flex;
}

.info-bar-alt section{
    width: 400px;
}
.info-bar-alt div{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    max-width: 1100px;
}
.info-bar-alt p{
    color: #435264;
    font-size: large;
    display: flex;
    align-items: center;
}

.info-bar-alt p img{
    margin-right: 10px;
}

.info-bar-alt h2{
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
.navbar-alt{
    display: flex;
    flex-flow: column;
    width: 100%;
    justify-content: center;
    align-items: center;
    /* height: 100px; */
    background-color: white;
    transition: 0.4s;
}

.transbg{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    z-index: 99;
    border-bottom: #bcc8d6 0.5px solid;
}

.backdrop-blur {
  background-color: rgba(255, 255, 255, .9);
}

/* if backdrop support: very transparent and blurred */
@supports ((-webkit-backdrop-filter: none) or (backdrop-filter: none)) {
  .backdrop-blur {
    background-color: rgba(255, 255, 255, .5);
    -webkit-backdrop-filter: blur(2em);
    backdrop-filter: blur(2em);
  }
}

.sticky {
  position: fixed;
  top: 0;
  width: 100%;
height: 90px;

}

.incpadding{
    margin-bottom: 150px;
}

.navbar-content-alt{
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

.nav-links a{
    font-size: x-large;
    font-weight: bold;
}

@media screen and (max-width: 800px){
    .nav-links{
        display: none;
    }

    .mobile-bar{
        display: flex;
        margin-bottom: 20px;
    }

    .info-bar-alt{
        display: none;
    }
}

</style>