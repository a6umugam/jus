<template>
  <div>
      <NavBarAlt :isFr="true"/>
      <div class="container">
          <div class="about-container">
                <h1 style="margin:20px">Que <strong>proposons-nous ?</strong></h1>
                <lottie-player src="https://assets5.lottiefiles.com/packages/lf20_tjrlxjj9.json"  background="transparent"  speed="1"  style="width:500px"  loop autoplay></lottie-player>
        <img style="width:50%;z-index:-2" src="~/assets/plus_line.svg" alt="plus">

              <div class="cards-holder">
                <Card :red="true" :long="true" :iconData="'globe'" :titleData="'Conception de site Web'" :textData="'Comprendre le contenu et la structure est un aspect clé de la conception Web. Conception de site Web réactif - une conception qui s’adapte à chaque écran. Nous avons la meilleure conception de site Web; nous voulons que votre site Web attire plus de trafic.'"/>
                <Card :purple="true" :long="true" :iconData="'lens'" :titleData="'Conception et développement de logiciels'" :textData="'Nous pouvons vous aider à concrétiser votre logiciel idéal. Nous intégrons les meilleurs logiciels pour faciliter l’édition. Générez des rapports de données en un seul clic.'"/>
                <Card :green="true" :long="true" :iconData="'mobile'" :titleData="'Développement d’applications mobiles/Web'" :textData="'Applications Web et mobiles conviviales. Nous concevons des applications parfaites, pour tous types d’appareils: Android et iOS.'"/>

                <Card :green="true" :long="true" :iconData="'card'" :titleData="'Prix abordables'" :textData="'Nous offrons des solutions haut de gamme et à des tarifs abordables. Nous sommes accessibles aux propriétaires de petites et moyennes entreprises. Contactez-nous pour un devis gratuit sur votre prochain projet.'"/>
                <Card :red="true" :long="true" :iconData="'film'" :titleData="'Production vidéo'" :textData="'Nous affichons la mission de votre entreprise ou de votre organisation à but non lucratif et faisons la promotion de produits et d’idées avec des vidéos ou animations.'"/>

                <Card :purple="true" :long="true" :iconData="'cart'" :titleData="'Commerce électronique'" :textData="'Notre solution est conçue pour faciliter le processus de gestion et d’exploitation de votre boutique en ligne.'"/>
                <Card :red="true" :long="true" :iconData="'award'" :titleData="'Développement et maintenance du site Web'" :textData="'Si votre site Web est obsolète et ne prend plus en charge votre marque, nous vous aiderons ! Une surveillance régulière de votre site Web est indispensable au bon fonctionnement de votre entreprise.'"/>
                <Card :purple="true" :long="true" :iconData="'face'" :titleData="'Image de marque et conception de logo'" :textData="'Nous nous engageons à fournir des designs 100% uniques et innovants à nos clients. Notre logo personnalisé vous aidera sûrement à trouver une identité commerciale réussie sur le marché.'"/>

                <Card :green="true" :long="true" :iconData="'layout'" :titleData="'Interfaces simples'" :textData="'Nos solutions sont simples à appliquer. Tout ce dont vous avez besoin est un accès à Internet, vous permettant d’apporter des modifications où que vous soyez.'"/>
                <Card :green="true" :long="true" :iconData="'heart'" :titleData="'Marketing des médias sociaux'" :textData="'Notre équipe conçoit et développe des campagnes de médias sociaux efficaces et engageantes pour nos clients, afin qu’ils promeuvent leur entreprise et atteignent leur audience cible.'"/>
                <Card :red="true" :long="true" :iconData="'chart'" :titleData="'Marketing de contenu'" :textData="'Nous avons une approche collaborative. Nous respectons vos idées, tout en déployant simultanément votre contenu, pour répondre au marché cible.'"/>
                <Card :purple="true" :long="true" :iconData="'flash'" :titleData="'Assistance informatique à distance'" :textData="'Nous adaptons les systèmes informatiques de votre entreprise selon vos besoins, en fournissant et en appliquant les meilleures solutions de maintenance. Ainsi, vous pouvez vous concentrer sur ce que vous faites le mieux.'"/>
                
        </div>


        <div class="space"></div>
        <div class="end-card">
            <h1 >Créons ensemble !</h1>
            <button v-on:click="goto('/contact')" style="font-size: x-large;">Obtenez un devis gratuit maintenant</button>
        </div>
        </div>
      </div>
        <!-- <div class="space"></div> -->
      <Footer :textData="'Chaque entreprise a besoin d’une forte présence en ligne pour être compétitive sur le marché actuel.'"/>
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