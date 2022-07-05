<template>
  <div>
      <Navbar/>
      <div class="container">
          
        <div class="about-container">

        <h2 style="color:#A2B8D2; margin-top:20px">Get In Touch</h2>
        <h1>Gatineau Web Solutions<br> Company</h1>
        <br>
        <p class="about-container-sub">Do you have a project in mind that you
                                      wish to discuss with our expert? Don't
                                      hesitate, we are just a call away! If you
                                      are unable to call us, you can just fill in
                                      the simple form below and we will get
                                      in touch with you as soon as possible.</p>

        <div class="space"></div>

    <ContactForm />


        <div class="contact-holder">
            <!-- <div class="contact">
                <img src="~/assets/icons/map.svg" alt="people">
                <h2>Location</h2>
                <p>207 Blank Street, Sample 407 Ottawa, ON K2P 2N2, Canada</p>
            </div> -->
            <div class="contact">
                <img src="~/assets/icons/phone.svg" alt="people">
                <h2>Need help right now?</h2>
                <p>Call: +1 (514) 292-3162</p>
            </div>
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

.about-container-sub{
    text-align: center;
  color: #5d6a79;
  font-size: large;
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