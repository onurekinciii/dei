<template>
  <div class="bg">
    <div class="banner">
        <div class="navbar">
          <img src="./assets/logo.png" class="logo">
          <h4 class="elcapi1">
            <strong :style="[flc]">D</strong>esignable
            <strong :style="[flc]">E</strong>conomic
            <strong :style="[flc]">I</strong>ndicators
          </h4>
          <ul>
            <li><a class="#">Home</a></li>
            <li><a class="#">About</a></li>
            <li><a class="#">Content</a></li>
            <li><a class="#">Sign In</a></li>
            <li><a class="#">Sign Up</a></li>
          </ul>
        </div>
    </div>
    <h4 class="elcapi2">
      Benefit from a panel service where you can
      <strong class="elcapi2 strong" style="color:red;">choose</strong> any type of graphic
      <strong class="elcapi2 strong" style="color:red;">and design it</strong> easily.
    </h4>
    <h1>awdawdwad</h1>
</div>
</template>

<script>
import test from './components/test.vue'

export default {
  components :{
    test
  },
  data(){
    return {
      currentTab: 'test',
      tabs: ['test']
  }
}
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  font-family: sans-serif;
}
.graph{
  margin: 60px 0px 0px 50px;
}
/*@font-face {
    font-family: NeogreyRegular;
    src: url("../assets/neuropolitical/neogrey/NeogreyMedium.otf") format("opentype");
}*/
@import url('https://fonts.googleapis.com/css2?family=Cinzel');
/*Navbar*/
.bg{
  width: 100%;
  height: 100vh;
  background-position: center;
  background-size: cover;
  background-image: linear-gradient(rgba(0,0,0,0.75),rgba(0,0,0,0.75)),url("https://imagevars.gulfnews.com/2018/11/25/181125_dow_jones_graph_resources1_16a08524268_large.jpg");
}
.navbar{
  width: 85%;
  margin: auto;
  padding: 9px 0;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.banner {
  background-color: #105b6e;
  border-bottom-left-radius: 50px;
  border-bottom-right-radius: 50px;
  height: 100px;
}
.logo{
  width: 80px;
  cursor: pointer;
}
.navbar ul li {
  list-style: none;
  display: inline-block;
  margin: 0 20px;
  position: relative;
}
.navbar ul li a{
  font-family: 'Cinzel', serif;
  font-weight: bold;
  text-decoration: none;
  color: black;
  text-transform: uppercase;
}
.navbar ul li::after{
  content: '';
  height: 3px;
  width: 0;
  background: #220608;
  position: absolute;
  left: 0;
  bottom: -5px;
  transition: 0.5s;
}
.navbar ul li:hover::after{
  width: 100%;
}

.elcapi1{
  margin: 0px 0px 0px -350px;
  font-family: 'Cinzel', serif;
  text-align: center;
}
.elcapi2{
  font-family: 'Cinzel', serif;
  text-align: left;
  letter-spacing: 1;
  margin-top: 40px;
  color : white;
}
.elcapi2:not(.strong){
  margin-left: 75px;
}
</style>
