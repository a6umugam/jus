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
              <a class="alt-button" href="/indexen"><img src="~/assets/icons/language-solid.svg" alt="lang" width="28">English</a>
          </div>
      </div>
      </div>

      <div class="mobile-bar">
        <section>
            <a href="/services">Nos Services</a>
            <a href="/about">À propos</a>
            <a href="/contact">Contact</a>
        </section>
        <div class="line"></div>
        <section>
            <button v-on:click="goto('/contact')" >Devis gratuit</button>
            <a href="/indexen" class="alt-button"> <img src="~/assets/icons/language-solid.svg" alt="lang" width="28"> English</a>
        </section>
        <div class="line"></div>
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
              <a href="/" class="alt-button"> <img src="~/assets/icons/language-solid.svg" alt="lang" width="28"> Français</a>
          </div>
      </div>
      </div>

      <div class="mobile-bar">
        <section>
            <a href="/servicesen">Services</a>
            <a href="/abouten">About</a>
            <a href="/contacten">Contact</a>
        </section>
        <div class="line"></div>
        <section>
            <button v-on:click="goto('/contacten')" >Free Quote</button>
            <a href="/" class="alt-button"> <img src="~/assets/icons/language-solid.svg" alt="lang" width="28"> Français</a>
        </section>
        <div class="line"></div>
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

.alt-button{
    margin-left: 10px;
    border: 1.5px solid #d3d3d3;
    border-radius: 10px;
    padding: 9px 7px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 125px;
    background-image: linear-gradient( 114.2deg,  #FFDEE9 22.6%, rgba(255,180,239,1) 67.7% );
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
    max-width: 1300px;
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
    /* background-color: #0f171f; */
    flex-flow: column;
    width: 100%;
    justify-content: center;
    height: 100px;
    align-items: center;
    display: none;
}

.mobile-bar section{
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    width: 100%;
    padding: 5px;
}

.line{
    width: 100%;
    border-bottom: #bcc8d6 0.5px solid;
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
    max-width: 1300px;
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

    .nav-buttons{
        display: none;
    }

    .mobile-bar{
        display: flex;
        /* margin-bottom: 20px; */
    }

    .info-bar-alt{
        display: none;
    }
}

</style>