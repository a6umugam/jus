<template>
  <div>
    <Navbar/>
    <Hero/>
    <Footer :textData="'Once your website is launched, we can continue to care for it. With our maintenance plan, You can send us fresh content, images or request layout changes at anytime. '"/>
  </div>
</template>

<script>
import Hero from "../components/Hero.vue";
import Navbar from "~/components/Navbar.vue";
import Footer from "~/components/Footer.vue";
export default {
    name: "IndexPage",
    components: { Hero, Navbar, Footer }
}
</script>

<style>

</style>