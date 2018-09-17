<template>
   <footer> 
        <div class="copyright">
        <p>&copy 2018 - Organization |
         <button @click="aboutUs">About Us |</button>
         <button @click="contactUs">Contact Us</button>
        </p>
        </div>
  </footer> 
</template>

<script>
export default {
  name: 'Footer',
  data () {
    return {
      
    }
  },
  methods:{
    contactUs(){
      this.$router.push({name: 'contact'})
    },
     aboutUs(){
      this.$router.push({name: 'about'})
    }
  }  
}
</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Raleway);
footer {

    
    background-color: rgba(22, 22, 22, 0.4);
    border-top: 3px solid rgba(0, 0, 0, 0.4);
    text-align:center;
    padding:20px;
   
    font-size: 1.4em;
    position: absolute;
    left: 0;
    bottom: 0;
    height: 60px;
    width: 100%;

     margin-left: 10px;
    
}
footer .copyright {
  width: 50%;
  float: left;
};
footer .copyright p {
  padding-left: 10%;
  color: white;
  font-size: 0.7em;
  line-height: 70px;
  text-transform: capitalize;
  letter-spacing: 1px;
}
.button{
  float: right;
  line-height: 150px;
  font-size: 1.4em;
}
</style>
