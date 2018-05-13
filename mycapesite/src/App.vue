<template>
  <div id="app">
      <header>
      <img src="./assets/capeLogo.png" alt="capelogo" id="logo">
      <h1>Duke University CAPE Program</h1>
      <ul id="navbar">
          <li class="option">Meet the Students</li>
          <li class="option">Meet the Leaders</li>
          <li class="option">CAPE Curriculum</li>
          <li class="option">Join CAPE</li>
          <li class="option">Donate</li>
        </ul>
          </header>
      <hr/>
      <h4>CAPE (Collegiate Athlete Pre-Medical Experience) is a year-round program offered by Duke University Medical Center to female student-athletes on Duke University's twelve collegiate varsity athletic teams. The program provides participants with a wide variety of clinical experiences that provide exposure to the world of Medicine. CAPE is designed to engage some of the nation's highest achieving young women in medical science and to assist them toward careers in Medicine.
        </h4>
      <div>
        <img class="mainpics" src="./assets/fhock.png" alt="fieldhockey">
          <img class="mainpics" src="./assets/soccer.png" alt="soccer">
          <img class="mainpics" src="./assets/trophy.png" alt="womanwithtrophy">
          </div>
      <q>We’re helping to change medicine a little bit and grow amazing young women into amazing doctors.</q>
      <p id="name">Terry Kruger</p>
      <p>Associate Director, CAPE</p>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
    methods:{
    
        meetStudents(){
            
        },
        meetLeaders(){
            
        },
        curriculum(){
            
        },
        join(){
            
        },
        donate(){
            
        },
    }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
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
    .option{
        border: solid thin black;
        padding: 5px;
    }
    .option:hover{
        cursor: pointer;
    }
    #logo{
        max-width: 20%;
        position: absolute;
        top: 5px;
        left: 5px;
    }
    .mainpics{
        max-width: 30%;
    }
    #name{
    }
    header{
/*
        background-image: url("./assets/header.jpg");
        background-size: cover;
*/
    }
</style>
