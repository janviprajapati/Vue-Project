<template>
  <div>
    <div>
    <Header></Header><br/><br/>
    </div>
    <div class="contain">
    <h1>{{ msg }}</h1>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from './Header.vue'
import Footer from './Footer.vue'
export default {
  name: 'HelloWorld',
 components:{
    Header,
    Footer,
 },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style scoped>
.contain{
  margin-top: 200px;
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
</style>
