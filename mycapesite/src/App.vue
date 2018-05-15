<template>
  <div id="app">
      <header>
      <img src="./assets/capeLogo.png" alt="capelogo" id="logo">
      <h1>Duke University CAPE Program</h1>
      <ul id="navbar">
            <li class="option" @click="home">Home</li>
          <li class="option" @click="meetStudents">Meet the Students</li>
          <li class="option" @click="meetLeaders">Meet the Leaders</li>
          <li class="option" @click="curriculum">CAPE Curriculum</li>
          <li class="option" @click="joinCape">Join CAPE</li>
          <li class="option" @click="donate">Donate</li>
        </ul>
          </header>
      <hr/>
      <div v-show="intro">
      <h4>CAPE (Collegiate Athlete Pre-Medical Experience) is a year-round program offered by Duke University Medical Center to female student-athletes on Duke University's thirteen collegiate varsity athletic teams. The program provides participants with a wide variety of clinical experiences that provide exposure to the world of Medicine. CAPE is designed to engage some of the nation's highest achieving young women in medical science and to assist them toward careers in Medicine.
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
      
      <div v-show="curr">
          <div id="currs">
          <div>
            <h2>School Year Curriculum</h2>
                <h3>Consultations</h3>
                    <p class="info">For one semester each year, students at the sophomore level and beyond shadow physicians as they perform new patient consultations at The Preston Robert Tisch Brain Tumor Center at Duke Medical Center. They learn the essentials of conducting a history and neurological examination, and very rapidly they are given primary responsibility as the first healthcare provider to see a new patient, take a history, do a neurological examination, and report to the attending physician.  
                    </p>
                <h3>Journal Club</h3>
                    <p class="info">At the monthly journal club meetings, CAPE students discuss assigned readings which address a broad span of issues in the medical field. 
                    </p>
                <h3>Role Model Dinner</h3>
                    <p class="info">The CAPE students host female medical students, housestaff, attending physicians and other healthcare providers.  They are given a real-world, rigorous exposure to the path they seek to follow.
                    </p>
                <h3>Leadership Sessions</h3>
                    <p class="info">CAPE students meet with leaders both inside and outside of Medicine to gain understanding of the skill sets necessary to develop and provide leadership in the medical, academic and community arenas.
                    </p>
              </div>
          <div>
          <h2>Summer Curriculum</h2>
                <h3>Internship</h3>
                    <ul class="list">
                        <li class="item">Between Sophomore and Junior Year</li>
                        <li class="item">Students rotate through the  clinical practices of CAPE faculty; participate in inpatient rounding, outpatient clinics, and any didactic sessions that occur during the students' time with their respective physicians
                        </li>
                        <li class="item">Those students who have a particular interest in laboratory work and who are 
                            considering careers as physician-scientists have the opportunity to intern in the laboratories of the CAPE basic science faculty</li>
                    </ul>
                <h3>Speakers</h3>
                    <ul class="list">
                        <li class="item">Weekly speakers every Friday</li>
                        <li class="item">Discuss a wide range of topics from ethical issues to career paths and objectives</li>
                        <li class="item">Women physicians specifically discuss balancing life as a physician and how to empower other women</li>
                    </ul>
                <h3>Teaching</h3>
                    <ul class="list">
                        <li class="item">CAPE Faculty teach weekly sessions</li>
                        <li class="item">Topics cover essentials of clinical medicine: history and physicals, specific diseases, symptom complexes </li>
                    </ul>
            </div>
              </div>
          </div>
              <div v-show="join">
                    <h2>Are you interested in joining the CAPE Program?</h2>
                  
                    <p>In order to be a member of cape you MUST fulfill the following requirements.</p>
                  <ul>
                    <li>You must be female</li>
                      <li>You must attend Duke University</li>
                      <li>You must be an undergraduate</li>
                      <li>You must be on one of the following Duke Varsity Women's Sports Teams
                        <ul>
                            <li>Women's Soccer</li>
                             <li>Women's Lacrosse</li>
                             <li>Women's Golf</li>
                             <li>Women's Tennis</li>
                            <li>Women's Basketball</li>
                            <li>Women's Volleyball</li>
                            <li>Women's Fencing</li>
                             <li>Swimming and Diving</li>
                             <li>Track and Field</li>
                             <li>Softball</li>
                            <li>Cross Country</li>
                            <li>Rowing</li>
                            <li>Field Hockey</li>
                            
                        </ul>
    
                        </li>
                </ul>
    
                </div>
    
  </div>
</template>

<script>
    //basketball cross-country fencing field hockey golf lacrosse rowing soccer softball swimming and diving tennis track and field volleyball
export default {
  name: 'app',
  data () {
    return {
      intro: true,
        meetS: false,
        meetL: false,
        curr: false,
        join: false,
        donate: false,
    
    }
  },
    methods:{
        home(){
           this.intro=true; 
            this.meetS=false;
            this.meetL=false;
            this.join=false;
            this.donate=false;
            this.curr=false;
        },
        meetStudents(){
            this.intro=false;
            this.meetS=true;
            this.meetL=false;
            this.join=false;
            this.donate=false;
            this.curr=false;
        },
        meetLeaders(){
            this.intro=false;
            this.meetS=false;
            this.meetL=true;
            this.join=false;
            this.donate=false;
            this.curr=false;
        },
        curriculum(){
            this.intro=false;
            this.meetS=true;
            this.meetL=false;
            this.join=false;
            this.donate=false;
            this.curr=true;
        },
        joinCape(){
            this.intro=false;
            this.meetS=false;
            this.meetL=false;
            this.donate=false;
            this.curr=false;
            this.join=true;
        },
        donate(){
            this.intro=false;
            this.meetS=false;
            this.meetL=false;
            this.join=false;
            this.donate=true;
            this.curr=false;
        },
    }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

a {
  color: #42b983;
}
    .option{
        border: solid thin black;
        padding: 5px;
        display: inline-block;
        margin: 0 10px;
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
    #currs{
        display: flex;
        justify-content: space-evenly;
    }

    .list{
        background-color: aliceblue;
        list-style-type: circle;
    }
    .item{
        text-align: left;
    }
    .info{
        text-align: left;
    }
</style>
