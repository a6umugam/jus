<template>
  <div class="contact-form">
    <form  @submit.prevent="submitForm">
    <label class="contact-email">
      <span>Email</span>
      <input placeholder="me@example.com" type="email" v-model="email" name="email">
    </label>
    <label class="contact-message">
      <span>Your Requirement / Query</span>
      <textarea name="message" v-model="message"></textarea>
    </label>
    <h3 v-if="errormsg" class="error-message">{{errormsg}}</h3>
    <button type="submit">Submit</button>
  </form>
  </div>
</template>

<script>
const FORMSPARK_ACTION_URL = "https://submit-form.com/QYsMCOVo";

export default {
  data() {
    return {
        errormsg:'',
        message: "",
        email:"",
    };
  },
  methods: {
    async submitForm() {
        if(this.message == ""){
            this.errormsg = "Please Enter Your Requirement / Query"
            return
        }
        var filter = /^([\w-]+(?:\.[\w-]+)*)@((?:[\w-]+\.)*\w[\w-]{0,66})\.([a-z]{2,6}(?:\.[a-z]{2})?)$/i
        if (filter.test(this.email)){
            await fetch(FORMSPARK_ACTION_URL, {
            method: "POST",
            headers: {
            "Content-Type": "application/json",
            Accept: "application/json",
            },
            body: JSON.stringify({
            message: this.message,
            email: this.email
            }),
        });
        alert("Form submitted");
        this.emitClose()
        }else{
            this.errormsg = "Please Enter A Valid Email"
        }
      
    },

    emitClose(){
        this.$emit('closeMenu')
    }
  },
};

</script>

<style>
.contact-form{
    display: flex;
    height: 100vh;
    width: 100vw;
    top: 0;
    position: fixed;
    justify-content: center;
    align-items: center;
    background-color: #00000073;
    padding: 10px;
}

.contact-form form{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-flow: column;
    background-color: white;
    border-radius: 12px;
    width: 100%;
    max-width: 600px;
    height: 500px;
    padding: 25px;
}

.contact-message{
    display: flex;
    flex-flow: column;
    height: 100%;
    width: 100%;
}

.contact-email{
    width: 100%;
    margin-bottom: 25px;
}

.contact-email input{
    width: 100%;
    height: 40px;
    border-radius: 10px;
    outline: none;
    border: 2px #686868 solid;
    padding: 5px;
    font-size: large;
}

.contact-form form label textarea{
    height: 100%;
    width: 100%;
    max-width: 550px;
    margin-bottom: 25px;
    border: 2px #686868 solid;
    border-radius: 10px;
    padding: 5px;
    font-size: large;
}   

.error-message{
    color: red;
    margin-bottom: 25px;
}
</style>