<template>
  <div>
      <NavBarAlt/>
      <div class="container">
          <div class="about-container">
                <h1 style="margin:20px">What do We <strong>Offer?</strong></h1>
                <lottie-player src="https://assets5.lottiefiles.com/packages/lf20_tjrlxjj9.json"  background="transparent"  speed="1"  style="width:500px"  loop autoplay></lottie-player>
        <img style="width:50%;z-index:-2" src="~/assets/plus_line.svg" alt="plus">

              <div class="cards-holder">
                <Card :red="true" :long="true" :iconData="'globe'" :titleData="'Website Design'" :textData="'Understanding the content and the structure is a key aspect of web design. Responsive Website Design – a design that adapts to every screen. We create the best website design; we want your website to attract more traffic.'"/>
                <Card :purple="true" :long="true" :iconData="'lens'" :titleData="'Software Design and Development'" :textData="'We can assist you in bringing to reality your ideal software. We integrate the best software to make it easy for anyone to edit. Generate data reports in just one simple click.'"/>
                <Card :green="true" :long="true" :iconData="'mobile'" :titleData="'Mobile / Web Application Development'" :textData="'User-friendly apps on both Android and iOS We build apps to look perfect across all device types. Dynamic web applications that are user-friendly.'"/>
                <Card :green="true" :long="true" :iconData="'card'" :titleData="'Cost-Effective'" :textData="'We offer high-end solutions and are accessible to small and medium business owners at affordable rates. Contact us for a free quote on your next project.'"/>
                <Card :red="true" :long="true" :iconData="'film'" :titleData="'Video Production'" :textData="'We display your business or nonprofit organization’s mission, and promote products and ideas with animated videos.'"/>
                <Card :purple="true" :long="true" :iconData="'cart'" :titleData="'E-commerce'" :textData="'Our solution is designed to ease the process of running and operating your online store.'"/>
                <Card :red="true" :long="true" :iconData="'award'" :titleData="'Website Development & Maintenance'" :textData="'If your website is out of date and no longer supports your brand, we will help you! Regular monitoring of your website is a must for keeping your business running smoothly.'"/>
                <Card :purple="true" :long="true" :iconData="'face'" :titleData="'Branding and Logo Design'" :textData="'We are committed to delivering 100% unique and innovative designs to our clients. Our customized logo will surely help you find a successful business identity in the market.'"/>
                <Card :green="true" :long="true" :iconData="'layout'" :titleData="'Simple Interfaces'" :textData="'Our solutions are simple to apply. All you need is access to the internet, enabling you to make changes from anywhere.'"/>
                <Card :green="true" :long="true" :iconData="'heart'" :titleData="'Social Media Marketing'" :textData="'Our team designs and develops effective, engaging social media campaigns for our clients to promote their business and reach their target audience.'"/>
                <Card :red="true" :long="true" :iconData="'chart'" :titleData="'Content Marketing'" :textData="'We use a collaborative approach to content creation and marketing. We respect your ideas while also simultaneously deploying your content to meet the target market.'"/>
                <Card :purple="true" :long="true" :iconData="'flash'" :titleData="'Remote IT Support'" :textData="'We subject your company’s IT systems to your needs by providing and applying the best maintenance solutions. So, you can focus on what you do best.'"/>
                
        </div>


        <div class="space"></div>
        <div class="end-card">
            <h1 >Let's create together!</h1>
            <button v-on:click="goto('/contact')" style="font-size: x-large;">Get Free Quotation Now</button>
        </div>
        </div>
      </div>
        <!-- <div class="space"></div> -->
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
    /* text-align: center; */
}

.about-container p{
    text-align: center;
  color: #5d6a79;
  font-size: large;
}


</style>