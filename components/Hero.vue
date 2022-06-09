<template>
  <div class="hero">
    <div class="hero-container">

        <div class="media-box">
            <video class="cover-image" autoplay loop>
                <source src="~/assets/wings_3d.mp4" type="video/mp4">
                Your browser does not support the video tag.
            </video> 
            <Slogan/>
        </div>

        <!-- <img class="cover-image" src="~/assets/jus-banner.jpg" alt="banner"> -->

        <!-- <p class="subtitle">We are a digital agency that focuses on
        solving your problems by making a product
        that will exceed your expectations so far</p> -->

    <div class="info-bar">
          <div>
            <h2>
              Website, Software & Mobile App
            </h2>

            <p>
              We pride ourselves on guiding our clients to success - and creating intelligent solutions that minimize risks and maximize rewards.
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
            We believe in designing solutions that make you money, but we also want
            to save you money by getting it done right the 1st time!
        </p>

        <div class="cards-holder">
            <div class="card">
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
            </div>
        </div>

        <!-- <div class="space"></div> -->


        <h1>Our Services</h1>
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

        </div>
        
        <a href="/services" class="o-button">More <img src="~/assets/icons/arrow.svg" alt=">" width="32"></a>


        <img class="cover-image" src="~/assets/jus_proc.jpg" alt="process">

        <a href="/services" class="o-button"><img src="~/assets/icons/email.svg" alt=">" width="32"> Lets Get Started</a>
        <div class="space"></div>
        <h1>Our Latest Project</h1>

        <div class="image-card">
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
        <div class="space"></div>


    </div>
  </div>
</template>

<script>
import Slogan from './Slogan.vue'
export default {

}
</script>

<style>

.media-box{
    display: flex;
    width: 90vw;
    justify-content: center;
    align-content: center;
    /* flex-flow: column; */
}

.o-button{
    border-radius: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 20px;
    border: 2px solid #F6F873;
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