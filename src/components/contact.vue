<template>
  <div>
      <div>
       <Header></Header><br/>
      </div>
      <div class="contain">
    <h1>{{ msg }}</h1>
      <section class="get-in-touch">
   <h1 class="title">Get in touch</h1>
   <form class="contact-form row">
      <div class="form-field col x-50">
         <input id="name" class="input-text js-input" type="text" required>
         <label class="label" for="name">Name</label>
      </div>
      <div class="form-field col x-50">
         <input id="email" class="input-text js-input" type="email" required>
         <label class="label" for="email">E-mail</label>
      </div>
      <div class="form-field col x-100">
         <input id="message" class="input-text js-input" type="text" required>
         <label class="label" for="message">Message</label>
      </div>
      <div class="form-field col x-100 align-center">
         <input class="submit-btn" type="submit" value="Submit">
      </div>
   </form>
</section>   
      </div>
      <div>
    <Footer></Footer>
    </div>
  </div>
</template>

<script>
import Header from './Header.vue'
import Footer from './Footer.vue'
export default {
  name: 'contact',
   components:{
    Header,
    Footer,
 },
  data () {
    return {
      msg: 'Welcome to contact us'
    }
  }
}
</script>

<style scoped>
@import url(https://fonts.googleapis.com/css?family=Raleway:300);
@import url(https://fonts.googleapis.com/css?family=Lusitana:400,700);
.contain{
    position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.align-center {
  text-align: center;
}
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

html {
  height: 100%;
}

body {
  height: 100%;
  position: relative;
}

.row {
  margin: -20px 0;
}
.row:after {
  content: "";
  display: table;
  clear: both;
}
.row .col {
  padding: 0 20px;
  float: left;
  box-sizing: border-box;
}
.row .col.x-50 {
  width: 50%;
}
.row .col.x-100 {
  width: 100%;
}
.get-in-touch .title {
  text-align: center;
  font-family: Raleway, sans-serif;
  text-transform: uppercase;
  letter-spacing: 3px;
  font-size: 36px;
  line-height: 48px;
  padding-bottom: 48px;
}

.contact-form .form-field {
  position: relative;
  margin: 32px 0;
}
.contact-form .input-text {
  display: block;
  width: 100%;
  height: 36px;
  border-width: 0 0 2px 0;
  border-color: #000;
  font-family: Lusitana, serif;
  font-size: 18px;
  line-height: 26px;
  font-weight: 400;
}
.contact-form .input-text:focus {
  outline: none;
}
.contact-form .input-text:focus + .label, .contact-form .input-text.not-empty + .label {
  -webkit-transform: translateY(-24px);
          transform: translateY(-24px);
}
.contact-form .label {
  position: absolute;
  left: 20px;
  bottom: 11px;
  font-family: Lusitana, serif;
  font-size: 18px;
  line-height: 26px;
  font-weight: 400;
  color: #888;
  cursor: text;
  transition: -webkit-transform .2s ease-in-out;
  transition: transform .2s ease-in-out;
  transition: transform .2s ease-in-out, -webkit-transform .2s ease-in-out;
}
.contact-form .submit-btn {
  display: inline-block;
  background-color: #000;
  color: #fff;
  font-family: Raleway, sans-serif;
  text-transform: uppercase;
  letter-spacing: 2px;
  font-size: 16px;
  line-height: 24px;
  padding: 8px 16px;
  border: none;
  cursor: pointer;
}
.note .link {
  color: #888;
  text-decoration: none;
}
.note .link:hover {
  text-decoration: underline;
}
</style>
