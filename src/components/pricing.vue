<template>
  <div>
       <Header></Header><br/>
    <h1>{{ msg }}</h1>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from './Header.vue'
import Footer from './Footer.vue'
export default {
  name: 'pricing',
   components:{
    Header,
    Footer,
 },
  data () {
    return {
      msg: 'Welcome to pricing'
    }
  }
}
</script>

<style scoped>
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
