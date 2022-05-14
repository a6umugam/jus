<template>
  <div>
      <Navbar/>
      <div class="container">
          <div class="about-container">
                <h1>What we offer</h1>

              <div class="cards-holder">
            <div class="card">
                <img src="~/assets/icons/award.svg" alt="people">
                <h2>Website development</h2>
                <p>We create websites that are optimized to drive results and convert your visitors. Find out how we can help.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/face.svg" alt="flash">
                <h2>Branding</h2>
                <p>The most memorable component of any business is their visual identity. Find out how we can help create one that sticks.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/bulb.svg" alt="flash">
                <h2>Email Marketing</h2>
                <p>Email marketing is a great way to maintain contact with visitors that are not ready to convert right away. Learn more here.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/flash.svg" alt="flash">
                <h2>Digital Marketing</h2>
                <p>With powerful advertising platforms available, FullView Design can help setup your campaigns and monitor long term results!</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/globe.svg" alt="flash">
                <h2>Video Production</h2>
                <p>Video is the best way to get your message across and increase time visitors spend on your website. Learn more about video services.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/layout.svg" alt="flash">
                <h2>Consulting</h2>
                <p>Have a strong marketing position and just need a little advice to accelerate your campaign? Our consulting services can help!</p>
            </div>

        </div>


        <div class="space"></div>
        <div class="end-card">
            <h1>Ready to<br>Work With Us!</h1>
            <button>Get Free Quotation Now</button>
        </div>
        </div>
      </div>
        <div class="space"></div>
      <Footer/>
  </div>
</template>

<script>
import Navbar from "~/components/Navbar.vue";
import Footer from "~/components/Footer.vue";
export default {
    components: { Navbar, Footer }
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
  color: #fff;
  font-size: large;
}
</style>