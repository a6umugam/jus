<template>
  <div class="hero">
    <div class="hero-container">
        <h2 style="font-weight:bold;font-style:italic;margin-top:20px">Promote your product or idea with animated videos</h2>
        <div class="media-box">
            <video class="cover-image" autoplay loop muted>
                <source src="~/assets/new_white_wings.webm" type="video/webm">
                Your browser does not support the video tag.
            </video> 
            <!-- <Slogan/> -->
        </div>

        <!-- <img class="cover-image" src="~/assets/jus-banner.jpg" alt="banner"> -->

        <!-- <p class="subtitle">We are a digital agency that focuses on
        solving your problems by making a product
        that will exceed your expectations so far</p> -->

        <h1 class="text-slogan">
            Full-service <strong>Web</strong> solutions to help your business<strong> grow!</strong>
        </h1>

    <div class="info-bar smooth-border">
          <div>
            <h2>
              Website, Software & Mobile App
            </h2>

            <p>
              We pride ourselves in guiding our clients to success - and creating intelligent solutions that minimize risks and maximize rewards.
            </p>
          </div>
    </div>

        <p class="subtitle">
            <!-- We are a forward thinking Gatineau web design company that produces
            beautiful optimized websites tailored to our clients individual business.
            Whether your need is a new website or a redevelopment, web updates or
            social media development and integration, we have the expertise and
            experience to get the job done right, quickly, and at a price you can afford.
            <br>
            <br>
            Our track record in providing superior products includes Logos, Branding,
            Web Design, Web &amp; App Development, we pretty much do it all.
            <br>
            <br> -->
            We believe in developing solutions that earn you money while saving
            you money. So we get the job done correctly from the get-go.
        </p>

        <div class="cards-holder">

        <div class="thecard">
            <div class="thefront">
                <img src="~/assets/icons/people.svg" alt="people">
                <h2>IT Expertise</h2>
                <img src="~/assets/icons/rotate.svg" style="width:18px" alt="people">
            </div>
            <div class="theback">
                <p>We have over 30 trained professionals in a range of technology areas. Our
                    goal is simple, to provide you with the best possible experience.</p>
            </div>
        </div>

        <div class="thecard">
            <div class="thefront">
                <img src="~/assets/icons/clock.svg" alt="people">
                <h2>24/7 Support</h2>
                <img src="~/assets/icons/rotate.svg" style="width:18px" alt="people">
            </div>
            <div class="theback">
                <p>We provide 24/7 support for all our valuable clients. If you
                    have any questions or run into any issues, we will reply within 30 minutes.</p>
            </div>
        </div>

        <div class="thecard">
            <div class="thefront">
                <img src="~/assets/icons/card.svg" alt="people">
                <h2>Affordable</h2>
                <img src="~/assets/icons/rotate.svg" style="width:18px" alt="people">
            </div>
            <div class="theback">
                <p>Our services are affordably priced and
                    budget-friendly. We do not overcharge our valuable clients.</p>
            </div>
        </div>

            <!-- <div class="card">
                <img src="~/assets/icons/people.svg" alt="people">
                <h2>IT Expertise</h2>
                <p>We have 20+ expert in our house. we will able to provide you 360° sservice as per your requirements</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/clock.svg" alt="flash">
                <h2>24/7 IT Support</h2>
                <p>We provide 24/7 support for our valuable clients. We will reply to all queries within 30 minutes.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/card.svg" alt="globe" >
                <h2>Affordable Cost</h2>
                <p>Our all service is affordable and budget friendly. We never overcharge our valuable clients. Any query just send a message.</p>
            </div> -->
        </div>

        <!-- <div class="space"></div> -->


        <!-- <h1>Our Services</h1>
        <p class="subtitle">We always provide an unforgettable service</p>

        <div class="cards-holder">
            <div class="card">
                <img src="~/assets/icons/bulb.svg" alt="people">
                <h2>Website Development</h2>
                <p>The core of our business, designing and developing custom websites for all industries, large and small.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/layout.svg" alt="flash">
                <h2>Responsive Websites</h2>
                <p>Designing for all platforms is a must today enhancing visitors experience on smart-phones, tablets and desktops.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/color.svg" alt="globe" >
                <h2>Print</h2>
                <p>Need print material for your next tradeshow, perhaps a booth designed? Maybe your menu needs a facelift.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/flash.svg" alt="globe" >
                <h2>Logos</h2>
                <p>Do you need a new logo? Don’t have a logo? We listen to our clients then create branding to suit your image. All branding is based around your logo.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/lens.svg" alt="globe" >
                <h2>SEO</h2>
                <p>In this day and age, people need to be able to find you. A well-optimized search engine friendly website will help reach more customers.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/globe.svg" alt="globe" >
                <h2>Website Hosting</h2>
                <p>We provide hosting for all of the websites we create, allowing you the peace of mind that we are only a phone call away.</p>
            </div>

        </div> -->
        
        <!-- <a href="/services" class="o-button">More <img src="~/assets/icons/arrow.svg" alt=">" width="32"></a> -->


        <img class="proc-image" src="~/assets/jus_proc_new2.png" alt="process">

        <button v-on:click="goto('/contact')"> Lets Get Started</button>
        <div class="space"></div>
        
        <!-- <h1>Our Latest Project</h1> -->

        <!-- <div class="image-card">
            <div>
                <img src="~/assets/statistic.jpg" alt="statistic-banner">
            </div>

            <div>
                <h2>Statistics Software</h2>
                <p class="subtitle">Desktop Software Dashboard</p>
            </div>
        </div>


        <div class="space"></div>
        <div class="end-card">
            <h1>Lets Discuss <br> For a Cool Project!</h1>
            <button>Get Free Quotation Now</button>
        </div>
        <div class="space"></div> -->

    <p class="subtitle">
        We have the <strong>resources, vision,</strong> and <strong>experience</strong> to design any
        website for any company with integrity and style. Our team of
        <strong>top web designers</strong> provides effective design solutions with
        <strong>attractive and functional</strong> features. These will meet, both your
        <strong>budget and deadline</strong> concerns.
    </p>

    </div>
  </div>
</template>

<script>
import Slogan from './Slogan.vue'
export default {
methods:{
        goto(path){
            this.$router.push(path)
        }
    }
}
</script>

<style>
.text-slogan{
    color: #181818;
    margin-bottom: 50px;
}

.text-slogan strong{
    font-weight: bolder;
    color: greenyellow;
}

.subtitle strong{
    font-weight: bolder;
    color: greenyellow;
}


.o-button{
    border-radius: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 20px;
    border: 2px solid greenyellow;
    padding: 10px 15px;
}

.o-button img{
    margin: 5px;
}

.image-card{
    display: flex;
    color: white;
    width: 100%;
    /* border: #213040 2px solid; */
    border-radius: 10px;
    padding: 25px 10px;
}

.image-card div{
    display: flex;
    flex-flow: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    text-align: center;
}

.image-card div img{
    width: 100%;
    border-radius: 10px;
}


.hero{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
}
.hero-container{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    max-width: 1100px;
    flex-flow: column;
    text-align: center;
}


@media screen and (max-width: 800px){

    .image-card{
        flex-flow: column;
    }
}
</style>