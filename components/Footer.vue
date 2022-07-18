<template>
  <div class="footer">
      <div class="footer-content">
          <section style="margin-right:110px">
              <!-- <a><strong>Office Location</strong></a> -->
              <a><img src="~/assets/icons/map_color.svg" width="28" alt="people"> Gatineau QC, <br> Canada</a>
              <a style="padding:5px"></a>
              <a><img src="~/assets/icons/phone_color.svg" width="28" alt="people"> +1 (514) 292-3162</a>
              <a style="padding:5px"></a>
              <a><img src="~/assets/icons/email_color.svg" width="28" alt="people"> info@jusmulticreation.ca</a>
          </section>

        <!-- <p class="bottom-text">
            
        {{textData}}
        <br> <br>
        {{altText}}

        </p> -->

  <div class="blockquote">
    <p>
      "{{textData}}"
        <br> <br>
        {{altText}}
     </p>
    <!-- <h4>&mdash;Steven Pressfield</h4> -->
  </div>

          <!-- <section>
              <h2>Services</h2>
              <a href="#">Social Media</a>
              <a href="#">Branding & UI/UX Design</a>
              <a href="#">FullStack Development</a>
          </section>

          <section>
              <h2>Contact</h2>
              <a href="#">WhatsApp</a>
              <a href="#">Telegram</a>
              <a href="#">Email</a>
          </section> -->
      </div>


      <div class="rights">
          <p>© 2022 JUS Multi Creation. All rights reserved.</p>
      </div>
  </div>
</template>

<script>
export default {
    props:{textData:'',altText:''},
}
</script>

<style>

/* Quote */
/* center the blockquote in the page */

/* Blockquote main style */
.blockquote {
    position: relative;
    font-family: 'Montserrat', sans-serif;
    font-weight: 800;
    color: #00ff40;
    padding: 30px 0;
    width: 100%;
    /* max-width: 500px; */
    z-index: 1;
    margin: 80px auto;
    align-self: center;
    border-top: solid 1px;
    border-bottom: solid 1px;
}

/* Blockquote header */
.blockquote p {
    position: relative;
    color: #000000;
    font-size: large;
    font-style: italic;
    /* font-weight: 800; */
    line-height: 1;
    margin: 0;
}

/* Blockquote right double quotes */
.blockquote:after {
    position: absolute;
    content: "”";
    color: #5a5a5a;
    font-size: 5rem;
    line-height: 0;
    bottom: -18px;
    right: 30px;
}

/* increase header size after 600px */
@media all and (min-width: 600px) {
    .blockquote p {
        font-size: 20px;
   }

}

/* Blockquote subheader */
/* .blockquote h4 {
    position: relative;
    color: #292a2b;
    font-size: 1.4rem;
    font-weight: normal;
    line-height: 1;
    margin: 0;
    padding-top: 20px;
    z-index: 1;
} */
/* Quote X */

.bottom-text{
    font-size: x-large;
    font-weight: bolder;
    font-style: italic;
}

.rights{
    margin-top: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 70px;
    color: white;
    background-color: #0f171f;
}
.footer{
    display: flex;
    flex-flow: column;
    width: 100%;
    justify-content: center;
    align-items: center;
    margin-top: 80px;
    font-size: larger;
}

.footer-content{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    max-width: 1100px;
}

.footer-content section{
    display: flex;
    flex-flow: column;
    max-width: 300px;
}

.footer-content section h2{
    color: white;
}

.footer-content section a{
    font-size: large;
    /* color: #5d6a79; */
    display: flex;
    align-items: flex-start;
    }

    .footer-content section a img{
    margin-right: 12px;
    }

@media screen and (max-width: 800px){
    .footer-content{
      flex-flow: column;
      justify-content: space-between;
      align-items: center;
      text-align: center;
      height: 400px;
    }
}
</style>