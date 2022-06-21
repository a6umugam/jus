<template>
  <div>
      <Navbar/>
      <div class="container">
          
          <div class="about-container">
        <div class="space"></div>
        <div class="space"></div>

                <h1>Coming Soon...</h1>

        <div class="space"></div>
             

        <div class="space"></div>
        <div class="end-card">
            <h1>Lets Discuss <br> For a Cool Project!</h1>
            <button v-on:click="formView = !formView" >Get Free Quotation Now</button>
        </div>
        </div>
      </div>
        <div class="space"></div>
      <Footer/>
      <ContactForm v-if="formView" @closeMenu="formView = !formView" />

  </div>
</template>

<script>
import Navbar from "~/components/Navbar.vue";
import Footer from "~/components/Footer.vue";
import ContactForm from "~/components/ContactForm.vue"

export default {
  data(){
        return{
            formView : false
    };
    },
    components: { Navbar, Footer,ContactForm }
}
</script>

<style>
.about-container{
    display: flex;
    width: 100%;
    max-width: 1100px;
    flex-flow: column;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.about-container p{
    text-align: center;
  color: #5d6a79;
  font-size: large;
}
</style>