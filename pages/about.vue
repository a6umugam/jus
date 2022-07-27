<template>
  <div>
      <NavBarAlt :isFr="true"/>
      <div class="container">
          <div class="about-container">
              <!-- <img class="cover-image" src="~/assets/jus-about.jpg" alt="creative"> -->

                <!-- <div class="space"></div> -->
                <h1 style="margin:20px"><strong>Entreprise</strong> de <strong>conception de site Web</strong> à Gatineau</h1>

        <!-- <img style="width:50%;z-index:-2" src="~/assets/plus_line.svg" alt="plus"> -->


                <div class="line-box">
                    <p style="text-align: start;font-size: x-large;"><strong>JUS Multi Creation est une entreprise canadienne de solutions Web, offrant des services digne de confiance.</strong>
                    <br><br>
                    - Nous fournissons une gamme de services
                    personnalisés, y compris la conception de sites
                    Web, le développement de logiciels et
                    d'applications, des vidéos d'animation et la
                    conception graphique, nous faisons à peu près tout.
                    <br><br>
                    - Notre équipe d'experts de haut niveau propose des
                    solutions de conception efficaces, attrayantes et
                    fonctionnelles, pouvant répondre à la fois à vos
                    préoccupations de budget et de délais. Nous
                    sommes là pour vous aider à franchir la prochaine
                    étape vers votre objectif !
                    <br><br>
                    <strong>JUS Multi Création s'engage à fournir des solutions
                    rentables et concentre ses services sur les
                    organismes communautaires et les nouveaux
                    entrepreneurs.</strong><br><br>
                    - Nous trouvons des moyens de rendre vos objectifs
                    atteignables, gérables et percutants.<br><br>
                    - Nos prestations de services, nos services à la
                    clientèle et notre politique d'entreprise visent à vous
                    offrir la meilleure expérience possible. N'hésitez pas
                    à nous contacter, nous serons heureux de vous
                    aider de toutes les manières possibles.
                    </p>
                </div>
        <img style="transform: scaleY(-1);width:40%;z-index:-2" src="~/assets/plus_line.svg" alt="plus">

        

              <h1>Nous nous <strong>soucions</strong> des <strong>résultats</strong> autant <strong>que vous !!!</strong></h1>

        <img style="width:40%;z-index:-2" src="~/assets/plus_line.svg" alt="plus">

              <div class="cards-holder">
            <div class="card">
                <img src="~/assets/icons/award.svg" alt="people">
                <h2>Services de haute qualité</h2>
                <p>Nous nous engageons à toujours vous apporter les
                meilleurs résultats ainsi que des solutions adaptées à
                vos projets.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/face.svg" alt="flash">
                <h2>Soutien amical</h2>
                <p>Nous avons une passion pour le design, nous aimons ce que nous faisons et nous savons que vous aimerez travailler avec nous.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/bulb.svg" alt="flash">
                <h2>Services aux entreprises créatives</h2>
                <p>Nous connaissons le design. Notre équipe
                créera un design unique, suivant votre vision et votre direction.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/flash.svg" alt="flash">
                <h2>Technologie la plus récente</h2>
                <p>Nous travaillons avec les toutes dernières technologies, ayant aussi les meilleures normes de l'industrie.</p>
            </div>

            <!-- <div class="card">
                <img src="~/assets/icons/globe.svg" alt="flash">
                <h2>Expand your reach</h2>
                <p>We build the tools and take it to market as well. Let us help generate traffic and increase conversions.</p>
            </div> -->

            <div class="card">
                <img src="~/assets/icons/layout.svg" alt="flash">
                <h2>Solutions réactives</h2>
                <p>Nos solutions ont fière allure et fonctionnent
                correctement sur tous les appareils et
                navigateurs.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/chart.svg" alt="flash">
                <h2>Des prix compétitifs</h2>
                <p>Nous offrons une remise spéciale aux groupes à
                but non lucratif et aux nouveaux entrepreneurs.</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/clock.svg" alt="globe" >
                <h2>Délais de livraison respectés</h2>
                <p>Nous ne voulons pas de retards, et vous non plus
                ? Une fois que tout est en place, nous pouvons démarrer votre projet et le terminer dans les délais convenus.</p>
            </div>
        </div>


        <div class="space"></div>
        <div class="end-card">
            <h2>Faisons équipe et créons ensemble</h2>
            <button v-on:click="goto('/contact')" style="font-size: x-large;">Obtenez un devis gratuit maintenant</button>
        </div>
        </div>
      </div>
        <div class="space"></div>
      <Footer :textData="'Nous sommes là pour vous aider à franchir la prochaine étape vers votre objectif.'"/>
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