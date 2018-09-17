<template>
  <div> 
    <div>
      <Header></Header><br/>
    </div>
    <div class="contain">
      <h1>{{ msg }}</h1>
      
      <h1>About us</h1>
      <p>Welcome to the [Company] website. My company believes that good financial decisions don't have to be confusing. I can provide simple, proven techniques that can help you make the most of your money and help achieve more of your financial goals.

This site will not only introduce you to my company philosophy and services, but it will also offer a wealth of educational materials, articles, newsletters, calculators, and other tools -- all designed to keep you up-to-date on financial issues, strategies, and trends. This educational material is updated frequently, as is our calendar of events, which lists upcoming financial workshops that you may want to attend.

If you have any questions or want to schedule a complimentary meeting to discuss your specific questions, you can e-mail me at (e-mail address) or call (phone number)..</p>
      
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
 name: 'about',
 components:{
    Header,
    Footer,
 },
  data () {
    return {
      msg: 'Welcome to about us'
    }

  }
}
</script>

<style>
.contain{
  /* margin-top: 200px; */
   position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
h1, h2 {
  font-weight: normal;
  align-content:flex-start;
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
</style>
