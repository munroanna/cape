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
          <li class="option" @click="donateHere">Donate</li>
        </ul>
          </header>
      <hr/>
      <div v-show="intro">
      <h4>CAPE (Collegiate Athlete Pre-Medical Experience) is a year-round program offered by Duke University Medical Center to female student-athletes on Duke University's thirteen collegiate varsity athletic teams. The program provides participants with a wide variety of clinical experiences that provide exposure to the world of Medicine. CAPE is designed to engage some of the nation's highest achieving young women in medical science and to assist them toward careers in Medicine.
        </h4>
          <p>If you would like to read more about CAPE, or download the complete information on CAPE you can read more <a href="file:///Users/annamunro/Desktop/cape/mycapesite/src/assets/CAPE_DONATION_FORM.pdf">here</a></p>
      <div>
        <img class="mainpics" src="./assets/fhock.png" alt="fieldhockey">
          <img class="mainpics" src="./assets/soccer.png" alt="soccer">
          <img class="mainpics" src="./assets/trophy.png" alt="womanwithtrophy">
          </div>
          <div id="quote">
          <q>We’re helping to change medicine a little bit and grow amazing young women into amazing doctors.</q>
      <p id="name">Terry Kruger</p>
      <p>Associate Director, CAPE</p></div><br>
          <div id="bigimag"><hr><br>
          <img src="./assets/Picture1.png" alt="womenandsports" id="womensports">
      </div>
          </div>
      <div v-show="meetL">
        
                <div id="direc" @click="showdirec"><hr/><h2>Directors</h2><hr/></div>
          <div v-show="dshow" id="alld">
          <div id="directors">
            <div class="dic">
            <h3>Henry S. Friedman, MD</h3>
            <h4>CO-DIRECTOR</h4>
            <ul class="dlist">
                <li>James B. Powell, Jr., Professor Neuro-Oncology</li>
                <li>Professor of Pediatrics</li>
                <li>Associate Professor of Surgery and Medicine</li>
                <li>Assistant Professor of Pathology</li>
                <li>Deputy Director, The Preston Robert Tisch Brain Tumor Center at Duke</li>
            </ul>
                <p>Henry S. Friedman, MD, is an internationally recognized neuro-oncologist with a career-long interest in the treatment of children and adults with brain and spinal cord tumors. He has written hundreds of articles on both the clinical and laboratory investigation of these neoplasms.
                </p>
                </div>
                        <div class="dic">
            <h3>Allan H. Friedman, MD</h3>
            <h4>CO-DIRECTOR</h4>
            <ul class="dlist">
                <li>The Guy L. Odom Professor of Neurological Surgery</li>
                <li>Deputy Director, The Preston Robert Tisch Brain Tumor Center at Duke</li>
                <li>Neurosurgeon-in-Chief, Duke University Hospital</li>
                <li>Program Director, Division of Neurosurgery/Department of Surgery</li>
            </ul>
                <p>Allan H. Friedman, MD, is an internationally recognized tumor and vascular neurosurgeon. He has a career-long interest in neuro-oncology, is responsible for over ninety percent of all tumor resections and biopsies conducted at Duke, and has written hundreds of articles on the neurosurgical management of brain tumors and vascular lesions. He is head of the Laboratory of Neurosurgical Oncology and an Associate Chief of the Preuss Laboratory for Brain Tumor Research.
                </p>
                </div>
        </div><br>
                      <div id="tk">
            <h3>Terry Kruger</h3>
            <h4>ASSOCIATE DIRECTOR</h4>
            <ul class="dlist">
                <li>University of Minnesota ’77,  Varsity Softball</li>
                <li>University of Minnesota Graduate School, MS</li>
            </ul>
                <p>Terry Kruger worked in adolescent therapy, crisis intervention, and was the Maui Island Director of the Girl Scouts before she came to Duke University in 2000. She has been the Associate Director of CAPE since its inception in 2005. She is responsible for the management, growth, and success of the program over the past six years.
                </p>
                </div></div>
          <div id="board">
                <div id="btitle" @click="showboard"><hr/><h2>Board of Advisors</h2>
              <hr/></div>
              <div v-show="bshow">
              <div id="exec">
              <h3>Executive Committee</h3>
              <h5>Chair- Sara Brandaleone </h5>
              <p>Retired Investment Banker, Philanthropist  </p>
              <h5>Bruce Brandaleone </h5>
              <p>Retired Investment Banker, Philanthropist  </p>
              <h5>George L. Grody</h5>
              <p>Retired, Global Strategic Alliance, Procter and Gamble</p>
                  </div>
              <br>
              <div id="cont">
              <div class="others">
              <h5>Johanna Bischof</h5>
              <p>CAPE, Duke Graduate, 2005, Duke University<br>MD 2010, Duke University<br>
                Emergency Medicine Resident,<br>
                Hennepin County Hospital, Minneapolis, MN
                </p>
              <h5>Larry Moneta, EdD</h5>
              <p>Vice President for Student Affairs, Duke University</p>
              <h5>Gwynn A. Young</h5>
              <p>Shareholder Carlton Fields, P. A., Tampa, Florida</p>
              <h5>Georgia Beasley</h5>
                 <p>Duke Graduate 2001, MD 2008,<br>
                Surgical Oncologist <br>
                     Duke University</p>
              <h5>Laura Gentile</h5>
              <p>Vice President, ESPN W</p>
                    </div>  
                  <div class="others">
              <h5>Scott McCune</h5>
              <p>Vice President Worldwide Sports<br>
                Entertainment and Media <br>
                The Coca-Cola Company<br>
                </p>
              <h5>Mark Emmert</h5>
              <p>President, NCAA</p>
              <h5>Kristina Johnson, PhD</h5>
              <p>Business Entrepreneur</p>
              <h5>Jean Spaulding, MD</h5>
              <p>Vice Chancellor for Health Affairs, Duke University </p>
              <h5>Kathryn Andolsek MD </h5>
              <p>Associate Director Graduate Medical Education 
                Duke University </p>
              <h5>Jacki Silar</h5>
              <p>Associate Athletic Director,  Duke University</p>
            </div>
            </div>
    </div></div>
        </div>
      <div v-show="curr">
          <div id="currs">
          <div class="cs" id="cs1">
            <h2>School Year Curriculum</h2>
                <h3 id="cons">Consultations</h3>
                    <p class="info">For one semester each year, students at the sophomore level and beyond shadow physicians as they perform new patient consultations at The Preston Robert Tisch Brain Tumor Center at Duke Medical Center. They learn the essentials of conducting a history and neurological examination, and very rapidly they are given primary responsibility as the first healthcare provider to see a new patient, take a history, do a neurological examination, and report to the attending physician.  
                    </p>
                <h3 id="club">Journal Club</h3>
                    <p class="info">At the monthly journal club meetings, CAPE students discuss assigned readings which address a broad span of issues in the medical field. 
                    </p>
                <h3 id="dinner">Role Model Dinner</h3>
                    <p class="info">The CAPE students host female medical students, housestaff, attending physicians and other healthcare providers.  They are given a real-world, rigorous exposure to the path they seek to follow.
                    </p>
                <h3 id="sess">Leadership Sessions</h3>
                    <p class="info">CAPE students meet with leaders both inside and outside of Medicine to gain understanding of the skill sets necessary to develop and provide leadership in the medical, academic and community arenas.
                    </p>
              </div>
          <div class="cs" id="cs2">
          <h2>Summer Curriculum</h2>
                <h3 id="intern">Internship</h3>
                    <ul class="list">
                        <li class="item">Between Sophomore and Junior Year</li>
                        <li class="item">Students rotate through the  clinical practices of CAPE faculty; participate in inpatient rounding, outpatient clinics, and any didactic sessions that occur during the students' time with their respective physicians
                        </li>
                        <li class="item">Those students who have a particular interest in laboratory work and who are 
                            considering careers as physician-scientists have the opportunity to intern in the laboratories of the CAPE basic science faculty</li>
                    </ul>
                <h3 id="speak">Speakers</h3>
                    <ul class="list">
                        <li class="item">Weekly speakers every Friday</li>
                        <li class="item">Discuss a wide range of topics from ethical issues to career paths and objectives</li>
                        <li class="item">Women physicians specifically discuss balancing life as a physician and how to empower other women</li>
                    </ul>
                <h3 id="teach">Teaching</h3>
                    <ul class="list">
                        <li class="item">CAPE Faculty teach weekly sessions</li>
                        <li class="item">Topics cover essentials of clinical medicine: history and physicals, specific diseases, symptom complexes </li>
                    </ul>
            </div>
              </div>
          </div>
              <div v-show="join">
                    <h2>Are you interested in joining the CAPE Program?</h2>
                  <div id="reqbox">
                    <p>In order to be a member of cape you MUST fulfill the following requirements.</p>
                  <ul id="req">
                    <li class="r">You must be female</li>
                      <li class="r">You must attend Duke University</li>
                      <li class="r">You must be an undergraduate</li>
                      <li class="r">You must be on one of the following Duke Varsity Women's Sports Teams
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
                      </div><br>
                  <hr/>
                  <p class="b">If you are a male, if you play on a club or recreational sport, if you attend a university other than Duke, or if you are NOT an undergraduate student, then unfortunately, you are not eligible for the CAPE program.</p>
                  <p class="b">However, if you fulfill the requirements above and are interested in joining CAPE, please contact Terry Kruger.</p>
                  <div id="contact">
                  <p>Terry Kruger<p>
                  <p>Email: terry.kruger@duke.edu</p>
                      </div>
    
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
        dshow: false,
        bshow: false
    
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
        donateHere(){
            this.intro=false;
            this.meetS=false;
            this.meetL=false;
            this.join=false;
            //this.donate=true;
            this.curr=false;
        },
        showdirec(){
            var changed=false
            if (this.dshow===true){
                this.dshow=false;
                changed=true;
            }
            if (this.dshow===false && changed===false){
                this.dshow=true;
            }
        },
        showboard(){
            var changed=false
            if (this.bshow===true){
                this.bshow=false;
                changed=true;
            }
            if (this.bshow===false && changed===false){
                this.bshow=true;
            }
    }
    }
}
</script>

<style lang="scss">
    body{
        background-color: lightgrey;
        background-image: url("./assets/grey3.jpg");
        color: black;
    }
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  text-align: center;
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
        list-style-type: circle;
    }
    .item{
        text-align: left;
    }
    .info{
        text-align: left;
    }
    #directors{
        display: flex;
        justify-content: space-evenly;
    }
    #womensports{
        max-width: 50%;
        border-style: groove;
        border-width: medium;
        border-color: antiquewhite
    }
    #quote{
        border: solid thin black;
        max-width: 60%;
        margin: 0 auto;
        background-color: lightyellow;
    }
    .dic{
        border: solid thin black;
        max-width: 40%;
        background-color: #EAEBEA;
    }
    #tk{
        border: solid thin black;
        max-width: 40%;
        margin: 0 auto;
        background-color: #EAEBEA;
    }
    #exec{
        border: solid thin darkred;
        max-width: 40%;
        margin: 0 auto;
    }
    .others{
        border: solid thin black;
        max-width: 35%;
        padding: 10px;
    }
    #cont{
        display: flex;
        justify-content: space-evenly;
    }
    #exec{
        color: darkred;
    }
    .cs{
        border: solid thin black;
        max-width: 48%;
        padding: 5px;
        color: aliceblue;
    }
    #cs1{
        background-color: #790339;
    }
    #cs2{
        background-color: #039C7D;
    }
    .dlist{
        list-style-type: none;
    }
    #req{
        list-style-type: decimal;
    }
    .r{
        text-align: left;
    }
    #reqbox{
        margin: 0 auto;
        max-width: 40%;
        border: solid medium darkblue;
        background-color: darkcyan;
        color: lightcyan;
        padding: 6px;
        
    }
    #contact{
        border: solid thin black;
        max-width: 40%;
        margin: 0 auto;
    }
    .b{
        font-weight: bold;
    }
    #direc{
        background-color: bisque;
        padding: 0;
        margin: 0;
    }
    #btitle{
        background-color: lightcoral;
    }
    #cons{
        background-color: #FA69AB;
    }
    #club{
        background-color: #FA69AB;
    }
    #dinner{
        background-color: #FA69AB;
    }
    #sess{
        background-color: #FA69AB;
    }
    #intern{
        background-color: royalblue;
    }
    #speak{
        background-color: royalblue;
    }
    #teach{
        background-color: royalblue;
    }
    h5{
        font-size: 12pt;
    }
    #bigimag{
        background-color: lightgrey;
    }
    #board{
        background-color: lightyellow;
        margin: 0;
    }
    #alld{
        background-color: #A5A2A0;
        margin: 0;
    }
</style>
