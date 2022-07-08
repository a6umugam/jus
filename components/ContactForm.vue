<template>
  <div class="contact-form">
    <form  @submit.prevent="submitForm">
    <label class="contact-email">
      <span>Name</span>
      <input  type="text" v-model="name" name="name">
    </label>
    <label class="contact-email">
      <span>Phone</span>
      <input  type="text" v-model="phone" name="phone">
    </label>
    <label class="contact-email">
      <span>Email</span>
      <input  type="text" v-model="email" name="email">
    </label>
    <label class="contact-message">
      <span>Message</span>
      <textarea name="message" v-model="message"></textarea>
    </label>
    <h3 v-if="errormsg" class="error-message">{{errormsg}}</h3>
    <button type="submit">Submit</button>
  </form>
  </div>
</template>

<script>
const FORMSPARK_ACTION_URL = "https://submit-form.com/NS3H4ss2";

export default {
  data() {
    return {
        errormsg:'',
        message: "",
        email:"",
        phone:'',
        name:''
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
              name:this.name,
              phone:this.phone,
              email: this.email,
              message: this.message,
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
    top: 0;
    /* position: fixed; */
    justify-content: center;
    /* align-items: center; */
    /* background-color: #00000073; */
    padding: 10px;
    width: 100%;

}

.contact-form form{
    display: flex;
    justify-content: flex-start;
    /* align-items: flex-start; */
    flex-flow: column;
    background-color: #eef6ff;
    border-radius: 12px;
    width: 100%;
    max-width: 600px;
    height: 600px;
    padding: 25px;
}

.contact-message{
    display: flex;
    flex-flow: column;
    height: 100%;
    width: 100%;
}


.contact-message span{
  display: flex;
  width: 100%;
}

.contact-email{
    width: 100%;
    margin-bottom: 25px;

}

.contact-email span{
  display: flex;
  width: 100%;
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