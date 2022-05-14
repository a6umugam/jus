<template>
  <div>
      <Navbar/>
      <div class="container">
          
          <div class="about-container">
        <div class="space"></div>
        <div class="space"></div>

                <h1>Coming Soon...</h1>

        <div class="space"></div>
             

        <div class="space"></div>
        <div class="end-card">
            <h1>Lets Discuss <br> For a Cool Project!</h1>
            <button>Get Free Quotation Now</button>
        </div>
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

.about-container p{
    text-align: center;
  color: #fff;
  font-size: large;
}
</style>