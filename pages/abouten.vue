<template>
  <div>
      <NavBarAlt/>
      <div class="container">
          <div class="about-container">
              <!-- <img class="cover-image" src="~/assets/jus-about.jpg" alt="creative"> -->

                <!-- <div class="space"></div> -->
                <h1 style="margin:20px"><strong>Web design</strong> company in <strong>Gatineau</strong></h1>

        <!-- <img style="width:50%;z-index:-2" src="~/assets/plus_line.svg" alt="plus"> -->


                <div class="line-box">
                    <p style="text-align: start;font-size: x-large;"><strong>JUS Multi Creation is a trusted full-service web solution company
                    based in Canada.</strong>
                    <br><br>
                    - We provide a range of customized services, including website
                    design, software and application development, animation
                    videos, and graphic design, we pretty much do it all.
                    <br><br>
                    - Our team of top experts offers effective design solutions that
                    are attractive, functional and can meet both your budget and deadline concerns. We are here to help you take the next step towards your goal !
                    <br><br>
                    <strong>JUS Multi Creation is committed to providing cost-effective solutions
                    and focuses its services on community-based organizations and
                    new entrepreneurs.</strong><br><br>
                    - We find ways to make your goals attainable, manageable, and
                    impactful.<br><br>
                    - Our service delivery, customer service, and company policy
                    are focused on providing you with the best possible
                    experience. Feel free to contact us, we will be happy to help in
                    any way we can.
                    </p>
                </div>
        <img style="transform: scaleY(-1);width:40%;z-index:-2" src="~/assets/plus_line.svg" alt="plus">

        

              <h1>We <strong>care</strong> about <strong>results</strong> as much <strong>as you do</strong> !</h1>

        <img style="width:40%;z-index:-2" src="~/assets/plus_line.svg" alt="plus">

              <div class="cards-holder">
            <div class="card">
                <img src="~/assets/icons/award.svg" alt="people">
                <h2>High-Quality Services</h2>
                <p>We are always committed to bring the best results and specialized outputs to your project.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/face.svg" alt="flash">
                <h2>Friendly Support</h2>
                <p>We have a passion for design, we love what we do and we know you will enjoy working with us.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/bulb.svg" alt="flash">
                <h2>Creative Business Services</h2>
                <p>Design is our specialty and our team will craft a unique creation
                reflective of your vision, while following your lead.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/flash.svg" alt="flash">
                <h2>Newest technology</h2>
                <p>We work with the very latest and greatest in industry standards and available technology.</p>
            </div>

            <!-- <div class="card">
                <img src="~/assets/icons/globe.svg" alt="flash">
                <h2>Expand your reach</h2>
                <p>We build the tools and take it to market as well. Let us help generate traffic and increase conversions.</p>
            </div> -->

            <div class="card">
                <img src="~/assets/icons/layout.svg" alt="flash">
                <h2>Responsive solutions</h2>
                <p>Our solutions look great and function properly on all devices and browsers.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/chart.svg" alt="flash">
                <h2>Competitive Pricing</h2>
                <p>We offer special discount for non-profit groups and new enterpreneurs.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/clock.svg" alt="globe" >
                <h2>On-time Delivery</h2>
                <p>We don’t want delays, and neither do you. Once
                everything is in place, we can start your project and finish it within the
                agreed time frame.</p>
            </div>
        </div>


        <div class="space"></div>
        <div class="end-card">
            <h2>Let us be part of your team <br> and let's create together!</h2>
            <button v-on:click="goto('/contacten')" style="font-size: x-large;">Get Free Quotation Now</button>
        </div>
        </div>
      </div>
        <div class="space"></div>
      <Footer :textData="'We are here to help you take the next step towards your goal.'"/>
      <!-- <ContactForm v-if="formView" @closeMenu="formView = !formView" /> -->

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
    methods:{
        goto(path){
            this.$router.push(path)
        }
    }
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
  color: #292929;
  font-size: large;
}
</style>