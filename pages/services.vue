<template>
  <div>
      <Navbar/>
      <div class="container">
          <div class="about-container">
                <h1>What we offer</h1>

              <div class="cards-holder">
            <div class="card">
                <img src="~/assets/icons/award.svg" alt="people">
                <h2>Website Development & Maintenance</h2>
                <p>We create websites that are optimized to drive results and convert your visitors. Find out how we can help.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/face.svg" alt="flash">
                <h2>Branding and Logo Design</h2>
                <p>The most memorable component of any business is their visual identity. Find out how we can help create one that sticks.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/bulb.svg" alt="flash">
                <h2>Content Marketing</h2>
                <p>marketing is a great way to maintain contact with visitors that are not ready to convert right away.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/flash.svg" alt="flash">
                <h2>Social Media Management</h2>
                <p>With powerful advertising platforms available, FullView Design can help setup your campaigns and monitor long term results!</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/globe.svg" alt="flash">
                <h2>Video Production</h2>
                <p>Video is the best way to get your message across and increase time visitors spend on your website. Learn more about video services.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/layout.svg" alt="flash">
                <h2>Creative Consulting</h2>
                <p>Have a strong marketing position and just need a little advice to accelerate your campaign? Our consulting services can help!</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/color.svg" alt="globe" >
                <h2>Print</h2>
                <p>Need print material for your next tradeshow, perhaps a booth designed? Maybe your menu needs a facelift.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/globe.svg" alt="globe" >
                <h2>Website Hosting</h2>
                <p>We provide hosting for all of the websites we create, allowing you the peace of mind that we are only a phone call away.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/layout.svg" alt="flash">
                <h2>IT Support</h2>
                <p>Have a strong position and just need a little advice to accelerate your tech? Our IT Support services can help!</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/color.svg" alt="globe" >
                <h2>Graphic Designing</h2>
                <p>The most memorable component of any business is their visual identity. Find out how we can help create one that sticks.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/flash.svg" alt="globe" >
                <h2>Ecommerce</h2>
                <p>Have a great idea of selling something online, Just let us help you with our Ecommerce support team.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/lens.svg" alt="globe" >
                <h2>Software and Application Development</h2>
                <p>We develop softwares and mobile applications for all size of companies.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/flash.svg" alt="globe" >
                <h2>Website Design</h2>
                <p>We create websites that are optimized to drive results and convert your visitors. Find out how we can help.</p>
            </div>

        </div>


        <div class="space"></div>
        <div class="end-card">
            <h1>Ready to<br>Work With Us!</h1>
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
    components: { Navbar, Footer, ContactForm },
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