<template>
  <div>
      <NavBarAlt :isFr="true"/>
      <div class="container">
          
        <div class="about-container">

        <h1 class="gradient-text" style="color:#2a5487;font-weight:1200">Entrer en contact</h1>
        <h1 > Solutions Web Gatineau<br> <strong>Compagnie</strong></h1>
        <!-- <div class="image-bg">
        <br>
        </div> -->

        <img class="cover-image" src="~/assets/gatineau.jpg" alt="">

        <div class="about-container-sub" >
        <lottie-player src="https://assets1.lottiefiles.com/packages/lf20_8tmvgkde.json"  background="transparent"  speed="1" style="cont-lottie"  loop autoplay></lottie-player>
        <p style="margin-top:20px;font-size:x-large;color:#000;padding:30px">Vous avez un projet en tête dont vous souhaiteriez discuter avec notre expert ? <br> N'hésitez pas à nous joindre : <strong>+1 (514) 292-3162</strong> <br><br> Si vous ne parvenez pas à nous appeler, vous pouvez remplir le formulaire ci-dessous. <br> Nous vous contacterons dès que possible.</p>

        </div>



        <!-- <div class="space"></div> -->

    <ContactForm :isFr='true' />


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
        <!-- <div class="space"></div> -->
      <Footer :textData="footerText" :altText="'Un guichet unique pour tous vos besoins en matière de portail, de Web et de marketing numérique, maintenant et à l’avenir. '"/>
  </div>
</template>

<script>
import NavBarAlt from "~/components/NavBarAlt.vue";
import Footer from "~/components/Footer.vue";
export default {
  data(){
    return{
      footerText: "Besoin de créer un outil ou une plateforme en ligne qui n'existe pas encore ? Nous pouvons aider."
    }
  },
    components: { NavBarAlt, Footer }
}
</script>

<style>

.cont-lottie{
  width:500px
}
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
  display: flex;
  justify-content: center ;
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

@media screen and (max-width: 800px){
  .about-container-sub{
    flex-flow: column;
    align-items: center;

  }

  .cont-lottie{width: 300px;}
}
</style>