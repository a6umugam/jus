<template>
  <div>
    <Navbar/>
    <Hero/>
    <Footer :textData="'Once your website is launched, we can continue to care for it. Our maintenance plan enables you to send us fresh content, and images or request layout changes at any time. '"/>
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