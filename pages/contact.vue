<template>
  <div>
      <Navbar/>
      <div class="container">
          
        <div class="about-container">

        <h2 style="color:#A2B8D2; margin-top:20px">Contact us</h2>
        <h1>Let's start somethig <br> big together.</h1>
        <br>
        <p class="about-container-sub">If you have any questions about or services or to find out more about how JUS Multi Creation can help your company get noticed please contact us via email or telephone.
            <br><br> We’re only a call away so make the next step in your digital success!</p>

        <div class="space"></div>

        <div class="contact-holder">
            <div class="contact">
                <img src="~/assets/icons/map.svg" alt="people">
                <h2>Location</h2>
                <p>207 Blank Street, Sample 407 Ottawa, ON K2P 2N2, Canada</p>
            </div>
            <div class="contact">
                <img src="~/assets/icons/phone.svg" alt="people">
                <h2>Phone</h2>
                <p>5142923162</p>
            </div>
            <div class="contact">
                <img src="~/assets/icons/email.svg" alt="people">
                <h2>Email</h2>
                <p>contact@justmulticreation.com</p>
            </div>
            <div class="contact">
                <img src="~/assets/icons/whatsapp.svg" alt="people">
                <h2>WhatsApp</h2>
            </div>
            <div class="contact">
                <img src="~/assets/icons/telegram.svg" alt="people">
                <h2>Telegram</h2>
            </div>
        </div>


        <div class="space"></div>

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