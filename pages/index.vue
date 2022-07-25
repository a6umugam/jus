<template>
  <div>
    <NavBarAlt :isFr="true"/>
    <HeroAltFr/>
    <Footer :textData="'Une fois votre site Web lancé, nous pouvons continuer à nous en occuper. Notre plan de maintenance vous permet de nous envoyer du nouveau contenu et des images ou de demander des changements de mise en page à tout moment.'"/>
  </div>
</template>

<script>
import HeroAltFr from "../components/HeroAltFr.vue";
import NavBarAlt from "~/components/NavBarAlt.vue";
import Footer from "~/components/Footer.vue";
export default {
    name: "IndexPage",
    components: { HeroAltFr, NavBarAlt, Footer }
}
</script>

<style>

</style>