<template>
  <div>
    <NavBarAlt/>
    <HeroAlt/>
    <Footer :textData="'Once your website is launched, we can continue to care for it. Our maintenance plan enables you to send us fresh content, and images or request layout changes at any time. '"/>
  </div>
</template>

<script>
import HeroAlt from "../components/HeroAlt.vue";
import NavBarAlt from "~/components/NavBarAlt.vue";
import Footer from "~/components/Footer.vue";
export default {
    name: "IndexPage",
    components: { HeroAlt, NavBarAlt, Footer }
}
</script>

<style>

</style>