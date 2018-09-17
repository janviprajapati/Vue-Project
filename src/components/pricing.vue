<template>
  <div>
    <div>
       <Header></Header><br/>
    </div>
    <div class="contain">
      <!-- <h1>{{ msg }}</h1> -->
      <div class="pricingtable">
      <div class="plan">
        <header>
          <h4 class="plan-title">
            Starter
          </h4>
          <div class="plan-cost"><span class="plan-price">$19</span><span class="plan-type">/month</span></div>
        </header>
        <ul class="plan-features">
          <li><i class="ion-checkmark"> </i>5GB Linux Web Space</li>
          <li><i class="ion-checkmark"> </i>5 MySQL Databases</li>
          <li><i class="ion-checkmark"> </i>Unlimited Email</li>
          <li><i class="ion-checkmark"> </i>250Gb mo Transfer</li>
          <li><i class="ion-checkmark"> </i>24/7 Tech Support</li>
          <li><i class="ion-checkmark"> </i>Daily Backups</li>
        </ul>
        <div class="plan-select"><button @click="Pricing">Select Plan</button></div>
      </div>
      <div class="plan">
        <header>
          <h4 class="plan-title">
            Basic
          </h4>
          <div class="plan-cost"><span class="plan-price">$29</span><span class="plan-type">/month</span></div>
        </header>
        <ul class="plan-features">
          <li><i class="ion-checkmark"> </i>10GB Linux Web Space</li>
          <li><i class="ion-checkmark"> </i>10 MySQL Databases</li>
          <li><i class="ion-checkmark"> </i>Unlimited Email</li>
          <li><i class="ion-checkmark"> </i>500Gb mo Transfer</li>
          <li><i class="ion-checkmark"> </i>24/7 Tech Support</li>
          <li><i class="ion-checkmark"> </i>Daily Backups</li>
        </ul>
        <div class="plan-select"><button @click="Pricing">Select Plan</button></div>
      </div>
      <div class="plan featured">
        <header>
          <h4 class="plan-title">
            Professional
          </h4>
          <div class="plan-cost"><span class="plan-price">$49</span><span class="plan-type">/month</span></div>
        </header>
        <ul class="plan-features">
          <li><i class="ion-checkmark"> </i>25GB Linux Web Space</li>
          <li><i class="ion-checkmark"> </i>25 MySQL Databases</li>
          <li><i class="ion-checkmark"> </i>Unlimited Email</li>
          <li><i class="ion-checkmark"> </i>2000Gb mo Transfer</li>
          <li><i class="ion-checkmark"> </i>24/7 Tech Support</li>
          <li><i class="ion-checkmark"> </i>Daily Backups</li>
        </ul>
        <div class="plan-select"><button @click="Pricing">Select Plan</button></div>
      </div>
      <div class="plan">
        <header>
          <h4 class="plan-title">
            Ultra
          </h4>
          <div class="plan-cost"><span class="plan-price">$99</span><span class="plan-type">/month</span></div>
        </header>
        <ul class="plan-features">
          <li><i class="ion-checkmark"> </i>100GB Linux Web Space</li>
          <li><i class="ion-checkmark"> </i>Unlimited MySQL Databases</li>
          <li><i class="ion-checkmark"> </i>Unlimited Email</li>
          <li><i class="ion-checkmark"> </i>10000Gb mo Transfer</li>
          <li><i class="ion-checkmark"> </i>24/7 Tech Support</li>
          <li><i class="ion-checkmark"> </i>Daily Backups</li>
        </ul>
        <div class="plan-select"><button @click="Pricing">Select Plan</button></div>
      </div>
      </div>
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
  name: 'pricing',
   components:{
    Header,
    Footer,
 },
  data () {
    return {
      // msg: 'Welcome to pricing'
    }
  },
   methods:{
    pricing(){
      this.$router.push({name: 'pricing'})
    }
}
}
</script>

<style scoped>
.contain{
  margin-top: 100px;
  position: fixed;
  top: 40%;
  left: 32%;
  transform: translate(-50%, -50%);
}
h1, h2 {
  font-weight: normal;
  text-align: center;
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


@import url(https://fonts.googleapis.com/css?family=Raleway:400,500,800);
@import url(https://fonts.googleapis.com/css?family=Montserrat:800);
.pricingtable {
  font-family: 'Raleway', Arial, sans-serif;
  color: #000000;
  text-align: center;
  font-size: 16px;
  width: 100%;
  max-width: 1000px;
  margin: 50px 50px 10px 500px;
}
.pricingtable .plan {
  margin: 0;
  width: 25%;
  position: relative;
  float: left;
  overflow: hidden;
  background-color: #e6e6e6;
  border: 5px solid #1e1e1e;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.3);
}
.pricingtable .plan:hover i,
.pricingtable .plan.hover i {
  -webkit-transform: scale(1.2);
  transform: scale(1.2);
}
.pricingtable * {
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  -webkit-transition: all 0.25s ease-out;
  transition: all 0.25s ease-out;
}
.pricingtable header {
  position: relative;
  background-color: #191919;
  color: #ffffff;
  padding: 20px 20px;
}
.pricingtable header:after {
  width: 0;
  height: 0;
  border-style: solid;
  border-width: 24px 150px 0 150px;
  border-color: #191919 transparent transparent transparent;
  content: '';
  position: absolute;
  top: 100%;
  left: 50%;
  -webkit-transform: translateX(-50%);
  transform: translateX(-50%);
}
.pricingtable .plan-title {
  top: 0;
  font-weight: 500;
  margin: 8px 0;
  text-transform: uppercase;
  font-weight: 400;
  letter-spacing: 1px;
}
.pricingtable .plan-cost {
  margin: 8px 0 0;
}
.pricingtable .plan-price {
  font-family: 'Montserrat', Arial, sans-serif;
  font-weight: 800;
  font-size: 2em;
  color: #ffffff;
}
.pricingtable .plan-type {
  opacity: 0.8;
  color: #ffffff;
  font-size: 0.7em;
  text-transform: uppercase;
}
.pricingtable .plan-features {
  padding: 40px 0 0;
  margin: 0;
  list-style: outside none none;
  font-size: 0.8em;
}
.pricingtable .plan-features li {
  border-top: 1px solid rgba(0, 0, 0, 0.2);
  padding: 10px 5%;
  font-weight: 500;
}
.pricingtable .plan-features li:nth-child(even) {
  background: rgba(0, 0, 0, 0.08);
}
.pricingtable .plan-features i {
  margin-right: 8px;
  opacity: 0.4;
}
.pricingtable .plan-select {
  border-top: 1px solid rgba(0, 0, 0, 0.2);
  padding: 20px;
}
.pricingtable .plan-select a{
  background-color: #1e1e1e;
  color: #ffffff;
  text-decoration: none;
  padding: 12px 20px;
  font-size: 0.75em;
  font-weight: 600;
  text-transform: uppercase;
  display: inline-block;
}
.pricingtable .plan-select a:hover {
  background-color: #2b2b2b;
}
.pricingtable .featured {
  margin-top: -10px;
  border: 5px solid #2b3c4e;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.3);
  z-index: 1;
}
.pricingtable .featured header {
  background-color: #222f3d;
}
.pricingtable .featured header:after {
  border-color: #222f3d transparent transparent transparent;
}
.pricingtable .featured .plan-select {
  padding: 30px 20px;
}
.pricingtable .featured .plan-select a {
  background-color: #222f3d;
}
@media only screen and (max-width: 767px) {
  .pricingtable .plan {
    width: 50%;
  }
  .pricingtable .plan-title,
  .pricingtable .plan-select a {
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }
  .pricingtable .plan-select,
  .pricingtable .featured .plan-select {
    padding: 20px;
  }
  .pricingtable .featured {
    margin-top: 0;
  }
}
@media only screen and (max-width: 440px) {
  .pricingtable .plan {
    width: 100%;
  }
}

body {
  background-color: whitesmoke;
}

</style>
