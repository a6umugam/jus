<template>
  <div>
      <Navbar/>
      <div class="container">
          <div class="about-container">
              <img class="cover-image" src="~/assets/jus-about.jpg" alt="creative">

                <div class="space"></div>
                <h1>About Us</h1>
                <p>We are specialists in web design, branding and logo design and search engine optimization. We help our clients stand out, generate leads and deliver results. Whether you’re a startup or an established company looking to expand—our team of highly talented individuals can help reach new heights. Visit our portfolio to see some of our latest projects and how we’ve helped our clients succeed with their digital marketing. Ready to make the next step? Contact us for an obligation free consult.</p>
        
                <div class="space"></div>

              <h1>Why Business Owners Love Working With Us !!</h1>

              <div class="cards-holder">
            <div class="card">
                <img src="~/assets/icons/award.svg" alt="people">
                <h2>High Quality Results</h2>
                <p>We are always committed to bring the best results and specialized outputs to your project.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/face.svg" alt="flash">
                <h2>We're friendly</h2>
                <p>Our team is friendly and easy to work with. We love what we do and we know you’ll enjoy working with us.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/bulb.svg" alt="flash">
                <h2>We're creative</h2>
                <p>We know design. Our team will craft a unique design based on your vision and direction.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/flash.svg" alt="flash">
                <h2>Newest technology</h2>
                <p>We work with the very latest and greatest in industry standards and available technology.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/globe.svg" alt="flash">
                <h2>Expand your reach</h2>
                <p>We build the tools and take it to market as well. Let us help generate traffic and increase conversions.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/layout.svg" alt="flash">
                <h2>Responsive solutions</h2>
                <p>Our solutions look great and function properly on all devices and browsers.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/chart.svg" alt="flash">
                <h2>Competitive Pricing</h2>
                <p>We offer top quality services with affordable pricing.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/clock.svg" alt="globe" >
                <h2>On-Time</h2>
                <p>We don’t want delays, and neither do you. Once everything is in place, we can start your project and finish it within the agreed period.</p>
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
    components: { Navbar, Footer, ContactForm }
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
    padding: 10px;
    text-align: center;
  color: #5d6a79;
  font-size: large;
}
</style>