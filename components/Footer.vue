<template>
  <div class="footer">
      <div class="footer-content">
          <section style="margin-right:110px">
              <p>Call Us : 514.292.3162</p>
              <p>info@jusmulticreation.ca</p>
          </section>

        <p>
        Once your website is launched, we can continue to care for it. With
        our maintenance plan, You can send us fresh content, images or
        request layout changes at anytime.
        </p>

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

}
</script>

<style>
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

.footer-content section p{
    font-size: large;
    color: #5d6a79;
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