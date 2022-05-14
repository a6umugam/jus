<template>
  <div class="hero">
    <div class="hero-container">
        <img class="cover-image" src="~/assets/jus-banner.jpg" alt="banner">

        <p class="subtitle">We are a digital agency that focuses on
        solving your problems by making a product
        that will exceed your expectations so far</p>

        <div class="space"></div>

        <h1>Our Services</h1>
        <p class="subtitle">We always provide an unforgettable service</p>

        <div class="cards-holder">
            <div class="card">
                <img src="~/assets/icons/people.svg" alt="people">
                <h2>Social Media</h2>
                <p>+ 150 Clients</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/flash.svg" alt="flash">
                <h2>Branding & UI/UX Design</h2>
                <p>+ 150 Clients</p>
            </div>

            <div class="card">
                <img src="~/assets/icons/globe.svg" alt="globe" >
                <h2>FullStack Developer</h2>
                <p>+ 150 Clients</p>
            </div>
        </div>

        <div class="space"></div>
        <h1>Our Latest Projects</h1>

        <div class="image-card">
            <div>
                <img src="~/assets/statistic.jpg" alt="statistic-banner">
            </div>

            <div>
                <h2>Statistics Software</h2>
                <p class="subtitle">Desktop Software Dashboard</p>
            </div>
        </div>

        <div class="image-card">
            <div>
                <h2>Statistics Software</h2>
                <p class="subtitle">Desktop Software Dashboard</p>
            </div>

            <div>
                <img src="~/assets/statistic.jpg" alt="statistic-banner">
            </div>

        </div>

        <div class="space"></div>
        <div class="end-card">
            <h1>Lets Discuss <br> For a Cool Project!</h1>
            <button>Get Free Quotation Now</button>
        </div>
        <div class="space"></div>


    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>


.image-card{
    display: flex;
    color: white;
    width: 100%;
    /* border: #213040 2px solid; */
    border-radius: 10px;
    padding: 25px 10px;
}

.image-card div{
    display: flex;
    flex-flow: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    text-align: center;
}

.image-card div img{
    width: 100%;
    border-radius: 10px;
}


.hero{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
}
.hero-container{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    max-width: 1100px;
    flex-flow: column;
    text-align: center;
}



@media screen and (max-width: 800px){

    .image-card{
        flex-flow: column;
    }
}
</style>