<template>
  <div>
      <NavBarAlt/>
      <div class="container">
          
        <div class="about-container">

        <h1 class="gradient-text" style="color:#2a5487;font-weight:1200">Get In Touch</h1>
        <h1 > Gatineau Web Solutions<br> <strong>Company</strong></h1>
        <!-- <div class="image-bg">
        <br>
        </div> -->

        <img class="cover-image" src="~/assets/gatineau.jpg" alt="">

        <p class="about-container-sub" style="margin-top:20px;font-size:x-large;color:#000;padding:30px">Do you have a project in mind you wish to discuss with our expert? <br> Feel free to reach out to us: <strong>+1 (514) 292-3162</strong> <br><br> If you are unable to call us, you can fill out the form below. <br> We will get in touch with you as soon as possible.</p>

        <!-- <div class="space"></div> -->

    <ContactForm />


        <div class="contact-holder">
            <!-- <div class="contact">
                <img src="~/assets/icons/map.svg" alt="people">
                <h2>Location</h2>
                <p>207 Blank Street, Sample 407 Ottawa, ON K2P 2N2, Canada</p>
            </div> -->
            <!-- <div class="contact">
                <img src="~/assets/icons/phone.svg" alt="people">
                <h2>Need help right now?</h2>
                <h2>Call: +1 (514) 292-3162</h2>
            </div> -->
            <!-- <div class="contact">
                <img src="~/assets/icons/email.svg" alt="people">
                <h2>Email</h2>
                <p>contact@justmulticreation.com</p>
            </div> -->
            <!-- <div class="contact">
                <img src="~/assets/icons/whatsapp.svg" alt="people">
                <h2>WhatsApp</h2>
            </div> -->
            <!-- <div class="contact">
                <img src="~/assets/icons/telegram.svg" alt="people">
                <h2>Telegram</h2>
            </div> -->
        </div>


        <!-- <div class="space"></div> -->

        </div>
      </div>
        <div class="space"></div>
      <Footer :textData="footerText" :altText="'A one-stop-shop for all your portal, web, and digital marketing requirements, now and in the future. '"/>
  </div>
</template>

<script>
import NavBarAlt from "~/components/NavBarAlt.vue";
import Footer from "~/components/Footer.vue";
export default {
  data(){
    return{
      footerText: "Need to build an online tool or platform that doesn't exist yet? We can help."
    }
  },
    components: { NavBarAlt, Footer }
}
</script>

<style>
.image-bg{
  background-image: url("~assets/gatineau.jpg");
  background-size: cover;
  padding: 20px;
  margin-top: 20px;
  border-radius: 10px;
  

}
.about-container{
    display: flex;
    width: 100%;
    max-width: 1100px;
    flex-flow: column;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.about-container-sub{
    text-align: center;
  color: #5d6a79;
  font-size: large;
  border: #eeeeee solid 1px;
  border-radius: 12px;
  padding: 20px;
}



.contact-holder{
  margin-top: 20px;
  display: flex;
  width: 100%;
  flex-wrap: wrap;
  justify-content: space-around;
}

.contact{
  display: flex;
  flex-flow: column;
  justify-content: space-around;
  width: 600px;
  height: 150px;
  background-color: #eef6ff;
  margin: 10px;
  padding: 10px;
  color: black;
  border-radius: 10px;
  transition: 0.5s;
}

.contact img{
  width: 50px;
}

.contact:hover{
  background-color: #F6F873;
  color: #000;
}
</style>