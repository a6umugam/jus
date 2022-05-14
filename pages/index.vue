<template>
  <div>
    <Navbar/>
    <Hero/>
    <Footer/>
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