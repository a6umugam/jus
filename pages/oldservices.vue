<template>
  <div>
      <NavBarAlt/>
      <div class="container">
          <div class="about-container">
                <h1>What do We <strong>Offer?</strong></h1>

              <div class="cards-holder">
                <Card :green="true" :long="true" :iconData="'people'" :titleData="'Expertise'" :textData="'experience'"/>
                <Card :purple="true" :long="true" :iconData="'globe'" :titleData="'Website Design'" :textData="'Understanding the content and the structure is a key aspect of web design. Responsive Website Design – a design that adapts to every screen. We create the best website design; we want your website to attract more traffic'"/>
                <Card :green="true" :long="true" :iconData="'award'" :titleData="'Website Development & Maintenance'" :textData="'If your website is out of date and no longer supports your brand, we will help you! Regular monitoring of your website is a must for keeping your business running smoothly.'"/>
                <Card :red="true" :long="true" :iconData="'people'" :titleData="'Expertise'" :textData="'experience'"/>
                <Card :red="true" :long="true" :iconData="'people'" :titleData="'Expertise'" :textData="'experience'"/>
                <Card :red="true" :long="true" :iconData="'people'" :titleData="'Expertise'" :textData="'experience'"/>
                <Card :red="true" :long="true" :iconData="'people'" :titleData="'Expertise'" :textData="'experience'"/>

                


            <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/award.svg" alt="people">
                <h2>Website Development & Maintenance</h2>
                </div>
                <div class="theback">
                <p>If your website is out of date and no longer supports your brand, we will
                help you! Regular monitoring of your website is a must for keeping your
                business running smoothly.</p>
                </div>
            </div>

            <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/face.svg" alt="flash">
                <h2>Branding and Logo Design</h2>
                </div>
                <div class="theback">
                <p>We are committed to delivering 100% unique and innovative designs to our
                    clients. Our customized logo will surely help you find a successful business
                    identity in the market.</p>
                </div>
            </div>

            
            <div class="thecard">
                <div class="thefront">
                    <img src="~/assets/icons/card.svg" alt="globe" >
                    <h2>Cost-Effective</h2>
                </div>
                <div class="theback">
                    <p>We offer high-end solutions and are accessible to small and medium
                        business owners at affordable rates. Contact us for a free quote on
                        your next project.</p>
                </div>
            </div>

            <div class="thecard">
                <div class="thefront">
                    <img src="~/assets/icons/layout.svg" alt="globe" >
                    <h2>Simple Interfaces</h2>
                </div>
                <div class="theback">
                    <p>Our solutions are simple to apply. All you need is access to the internet,
                        enabling you to make changes from anywhere.</p>
                </div>
            </div>

            <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/facebook.svg" alt="flash">
                <h2>Social Media Marketing</h2>
                </div>
                <div class="theback">
                <p>Our team designs and develops effective, engaging social media campaigns
                    for our clients to promote their business and reach their target audience.</p>
                </div>
            </div>

            <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/chart.svg" alt="flash">
                <h2>Content Marketing</h2>
                </div>
                <div class="theback">
                <p>We use a collaborative approach to content creation and marketing. We
                    respect your ideas while also simultaneously deploying your content to meet
                    the target market.</p>
                </div>
            </div>


            <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/film.svg" alt="flash">
                <h2>Video Production</h2>
                </div>
                <div class="theback">
                <p>We display your business or nonprofit organization’s mission, and promote products and ideas with animated videos.</p>
                </div>
            </div>

            <!-- <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/layout.svg" alt="flash">
                <h2>Creative Consulting</h2>
                </div>
                <div class="theback">
                <p>Have a strong marketing position and just need a little advice to accelerate your campaign? Our consulting services can help!</p>
                </div>
            </div> -->

            <!-- <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/color.svg" alt="globe" >
                <h2>Print</h2>
                </div>
                <div class="theback">
                <p>Need print material for your next tradeshow, perhaps a booth designed? Maybe your menu needs a facelift.</p>
                </div>
            </div> -->

            <!-- <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/globe.svg" alt="globe" >
                <h2>Website Hosting</h2>
                </div>
                <div class="theback">
                <p>We provide hosting for all of the websites we create, allowing you the peace of mind that we are only a phone call away.</p>
                </div>
            </div> -->

            <!-- <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/layout.svg" alt="flash">
                <h2>IT Support</h2>
                </div>
                <div class="theback">
                <p>Have a strong position and just need a little advice to accelerate your tech? Our IT Support services can help!</p>
                </div>
            </div> -->

            <!-- <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/color.svg" alt="globe" >
                <h2>Graphic Designing</h2>
                </div>
                <div class="theback">
                <p>The most memorable component of any business is their visual identity. Find out how we can help create one that sticks.</p>
                </div>
            </div> -->

            <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/cart.svg" alt="globe" >
                <h2>E-commerce</h2>
                </div>
                <div class="theback">
                <p>Our solution is designed to ease the process of running and operating your online store.</p>
                </div>
            </div>

            <div class="thecard">
                <div class="thefront">
                    <img src="~/assets/icons/flash.svg" alt="globe" >
                    <h2>Remote IT Support</h2>
                </div>
                <div class="theback">
                    <p>We subject your company's IT systems to your needs by providing and
                        applying the best maintenance solutions. So, you can focus on what you do best.</p>
                </div>
            </div>

            <div class="thecard">
                <div class="thefront">
                <img src="~/assets/icons/lens.svg" alt="globe" >
                <h2>Software Design and Development</h2>
                </div>
                <div class="theback">
                <p>We can assist you in bringing to reality your ideal software. We integrate the
                    best software to make it easy for anyone to edit. Generate data reports in just
                    one simple click</p>
                </div>
            </div>

            <div class="thecard">
                <div class="thefront">
                    <img src="~/assets/icons/mobile.svg" alt="globe" >
                    <h2>Mobile / Web Application Development</h2>
                </div>
                <div class="theback">
                    <p>User-friendly apps on both Android and iOS We build apps to look
                        perfect across all device types. Dynamic web applications that are
                        user-friendly.</p>
                </div>
            </div>

            

        </div>


        <div class="space"></div>
        <div class="end-card">
            <h1>Let's create together!</h1>
            <button v-on:click="goto('/contact')" >Get Free Quotation Now</button>
        </div>
        </div>
      </div>
        <div class="space"></div>
      <Footer :textData="'Every business needs a strong online presence to compete in the current marketplace.'"/>
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
    max-width: 1500px;
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