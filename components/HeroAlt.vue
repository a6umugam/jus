<template>
  <div class="hero">
    <div class="hero-container-alt">
        <ScrollText :textData="'Hwllow'"/>

        <!-- <h2 style="font-weight:bold;font-style:italic;margin-top:20px">Promote your product or idea with animated videos</h2> -->
        <div class="media-box">
            <video class="cover-image" autoplay loop muted>
                <source src="~/assets/new_white_wings.webm" type="video/webm">
                Your browser does not support the video tag.
            </video> 
            <!-- <Slogan/> -->
        </div>


            <div class="animation-promo" style="justify-content:center;padding:20px">
            
            <section class="text-place gradient-text">
                <p style="font-style:italic">
                Promote your product and idea with animated videos!
                </p>
            </section>

            </div>

        <img style="transform: scaleY(-1);width:20%;z-index:-2" src="~/assets/plus_line.svg" alt="plus">




        <!-- <img class="cover-image" src="~/assets/jus-banner.jpg" alt="banner"> -->

        <!-- <p class="subtitle">We are a digital agency that focuses on
        solving your problems by making a product
        that will exceed your expectations so far</p> -->

        <h1 class="text-slogan">
            "Full-service <strong>Web</strong> solutions to help your business<strong> grow</strong>"
        </h1>

        <img style="z-index:-2" src="~/assets/platforms.svg" alt="platforms">


        <img style="width:20%;z-index:-2" src="~/assets/plus_line.svg" alt="plus">


            <div class="text-place">
            <div>
                <div class="animation-promo">

            <section>
                <lottie-player src="https://assets4.lottiefiles.com/packages/lf20_x5jglqn9.json"  background="transparent"  speed="1"  class="lottie-anim"  loop autoplay></lottie-player>
            </section>                

            <section class="text-place gradient-text">
                <h1>
                Website, Software & Mobile App
                </h1>
            </section>

            </div>
            
                

                <h2 class="gradient-text" style="margin-top:20px">
                We pride ourselves in guiding our clients to success - and creating intelligent solutions that minimize risks and maximize rewards.
                </h2>
            </div>
            </div>

            
            

        <div class="mid-card gradi">

            <p class="subtitle" style="font-size:30px;text-align: start;max-width: 100%;font-family: 'Berkshire Swash', cursive;">
                We believe in developing solutions that earn you money while saving
                you money. So we get the job done correctly from the get-go.
            </p>

            <div class="cards-holder">

                <Card :red="true" :iconData="'people'" :titleData="'IT Expertise'" :textData="'We have over 30 trained professionals in a range of technology areas. Our goal is simple, to provide you with the best possible experience.'"/>
                <Card :purple="true" :iconData="'clock'" :titleData="'24/7 Support'" :textData="'We provide 24/7 support for all our valuable clients. If you have any questions or run into any issues, we will reply within 30 minutes.'"/>
                <Card :green="true" :iconData="'card'" :titleData="'Affordable'" :textData="'Our services are affordably priced and budget-friendly. We do not overcharge our valuable clients.'"/>

            <!-- <div class="thecard">
                <div class="thefront">
                    <img src="~/assets/icons/people.svg" alt="people">
                    <h2>IT Expertise</h2>
                    <section class="bottom-place">
                        <img src="~/assets/icons/rotate.svg" style="width:22px" alt="people">
                    </section>
                </div>
                <div class="theback">
                    <p>We have over 30 trained professionals in a range of technology areas. Our
                        goal is simple, to provide you with the best possible experience.</p>
                </div>
            </div> -->

            <!-- <div class="thecard">
                <div class="thefront">
                    <img src="~/assets/icons/clock.svg" alt="people">
                    <h2>24/7 Support</h2>
                    <section class="bottom-place">
                        <img src="~/assets/icons/rotate.svg" style="width:22px" alt="people">
                    </section>
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
                    <section class="bottom-place">
                        <img src="~/assets/icons/rotate.svg" style="width:22px" alt="people">
                    </section>
                </div>
                <div class="theback">
                    <p>Our services are affordably priced and
                        budget-friendly. We do not overcharge our valuable clients.</p>
                </div>
            </div> -->
            </div>
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

        <img class="proc-image" src="~/assets/jus_proc_new_one.png" alt="process">

        <button v-on:click="goto('/contact')" style="font-size: x-large;"> Lets Get Started</button>
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

    
    <div class="mid-card grey">
        <img src="~/assets/corner_design.svg" alt="corner">
        <p class="subtitle"  style="color: white;">
        We have the <strong>resources, vision,</strong> and <strong>experience</strong> to design any <br>
        website for any company with integrity and style. Our team of<br>
        <strong>top web designers</strong> provides effective design solutions with<br>
        <strong>attractive and functional</strong> features. These will meet, both your<br>
        <strong>budget and deadline</strong> concerns.
    </p>
    </div>

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

.animation-promo{
    width: 100%;
    max-width: 900px;
    display: flex;
    border: #eeeeee solid 1px;
    border-radius: 12px;
}

.animation-promo section{
    display: flex;
    align-items: center;
}

.animation-promo section p{
    font-size: xx-large;
    font-weight: bolder;
}

.lottie-anim{
    height: 400px;
    width: 400px;
}


.text-place{
    max-width: 900px;
}
.mid-card{
    padding: 20px;
    margin-top: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-flow: column;
    width: 90%;
    /* z-index: -2; */
    border-radius: 12px;
}

.mid-card img{
    position: absolute;
    width: 92%;
}

.gradi{
    background-image: linear-gradient( 112deg, #FFDEE9 0%, #B5FFFC 100%);

}

.grey{
    /* background-image: url("~assets/new_bg.svg"); */
    background-size: cover;
    background-position: bottom;
    background-color: #202020;
}

.text-slogan{
    color: #181818;
    margin-bottom: 50px;
    max-width: 1100px;
  background-image: url("~assets/new_bg.svg");
  background-size: cover;

}

.text-slogan strong{
    font-weight: bolder;
    color: greenyellow;
}

.subtitle strong{
    font-weight: bolder;
    color: greenyellow;
}

.media-box{
    display: flex;
    width: 70vw;
    justify-content: center;
    align-content: center;
    /* flex-flow: column; */
    margin-bottom: 50px;
    background-color: white;
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
.hero-container-alt{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    /* max-width: 1100px; */
    flex-flow: column;
    text-align: center;
    background-image: url("~assets/bubbles.svg");

}


.gradient-anim{
    background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
	background-size: 400% 400%;
	animation: gradient 15s ease infinite;
}




@media screen and (max-width: 800px){

    .image-card{
        flex-flow: column;
    }
}
</style>