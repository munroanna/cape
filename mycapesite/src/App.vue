<template>
  <div id="app">
      <header>
          <ul id="top">
      <li id="cape"><img src="./assets/capeLogo.png" alt="capelogo" id="logo"></li>
              <li id="htitle"><h1 id="big">Duke University CAPE</h1></li>
         <li id="dukie"><img src="./assets/duke.jpg" alt="dukelogo" id="duke"></li>
              </ul>
          </header>
      <div id="bod">
      <ul id="navbar">
            <li class="option" @click="home">Home</li>
          <li class="option" @click="meetStudents">Meet the Students</li>
          <li class="option" @click="meetLeaders">Meet the Leaders</li>
          <li class="option" @click="curriculum">CAPE Curriculum</li>
          <li class="option" @click="joinCape">Join CAPE</li>
          <li class="option" @click="donateHere">Donate</li>
        </ul>
      <hr/>
      <div v-show="intro">
      <h4 id="introex">CAPE (Collegiate Athlete Pre-Medical Experience) is a year-round program offered by Duke University Medical Center to female student-athletes on Duke University's thirteen collegiate varsity athletic teams. The program provides participants with a wide variety of clinical experiences that provide exposure to the world of Medicine. CAPE is designed to engage some of the nation's highest achieving young women in medical science and to assist them toward careers in Medicine.
        </h4>
          <p id="readmore">If you would like to read more about CAPE, or download the complete information on CAPE you can read more <a href="file:///Users/annamunro/Desktop/cape/mycapesite/src/assets/CAPE_DONATION_FORM.pdf">here</a></p>
      <div id="images">
          <img class="smaller" src="./assets/fhock.jpg" alt="fieldhockey">
          <img class="smaller" src="./assets/soccer.jpg" alt="soccer">
          <img class="smaller" src="./assets/trophy.jpg" alt="womanwithtrophy"></div>
          <div id="quote">
          <q>We’re helping to change medicine a little bit and grow amazing young women into amazing doctors.</q>
      <p id="name">Terry Kruger</p>
      <p>Associate Director, CAPE</p></div><br>
          </div>
          <div v-show="meetS">
            <ul id="studpics">
                <li><img src="./assets/img1.png">
                    <p class="blue">Johanna E. Bischof</p>
                    <p class="caption">Duke Undergraduate ’05
                    Duke Medical School ’10<br>
                    Field Hockey<br>
                    2003 Team Captain, All-America Selection<br>
                    EM Resident Hennepin County Hospital<br>
                    Attending ED physician,  Portland, OR
                    </p>
                </li>
                <li><img src="./assets/img2.png">
                    <p class="blue">Emily Waner</p><p class="caption">
                Duke Undergraduate ’08<br>
                Duke Medical School ’13<br>
                Basketball<br>
                Hospitalist <br>
                University of  Washington</p>
                </li>
                <li><img src="./assets/img3.png">
                    <p class="blue">Abby Johnston</p>
                        <p class="caption">CAPE Duke Undergraduate ’12<br>
                        Diving<br>
                        2x All-America Selection, USA Diving Team,  <br>
                        2012 Olympic Silver Medal <br>
                        Synchro Diving <br>
                        3nd  Year Duke Medical School<br>
                        2016 Olympian 3M Springboard<br>
                        </p>
                </li>
                <li><img src="./assets/img4.png">
                    <p class="blue">Elizabeth Williams</p>
                    <p class="caption">Duke Undergraduate ’15<br>
                    Basketball<br>
                    No. 1 High School Ranked Player<br>
                    WNBA <br>
                        Atlanta Dream</p>
                </li>
            </ul>
              <p id="whoare">CAPE participants are female student athletes from Duke University who have expressed interest in careers in Medicine.</p>
    
        </div>
      <div v-show="meetL">
        <div id="d">
                <div id="direc" @click="showdirec"><hr/><h2>Directors</h2><hr/></div>
          <div v-show="dshow" id="alld">
          <div id="directors">
            <div class="dic">
                <img src="./assets/henry.png" alt="henryheadshot" class="headshot">
            <h3>Henry S. Friedman, MD</h3>
            <h4>CO-DIRECTOR</h4>
            <ul class="dlist">
                <li>James B. Powell, Jr., Professor Neuro-Oncology</li>
                <li>Professor of Pediatrics</li>
                <li>Associate Professor of Surgery and Medicine</li>
                <li>Assistant Professor of Pathology</li>
                <li>Deputy Director, The Preston Robert Tisch Brain Tumor Center at Duke</li>
            </ul>
                <p class="des">Henry S. Friedman, MD, is an internationally recognized neuro-oncologist with a career-long interest in the treatment of children and adults with brain and spinal cord tumors. He has written hundreds of articles on both the clinical and laboratory investigation of these neoplasms.
                </p>
                </div>
                        <div class="dic">
            <img src="./assets/allan.png" alt="allanheadshot" class="headshot">
            <h3>Allan H. Friedman, MD</h3>
            <h4>CO-DIRECTOR</h4>
            <ul class="dlist">
                <li>The Guy L. Odom Professor of Neurological Surgery</li>
                <li>Deputy Director, The Preston Robert Tisch Brain Tumor Center at Duke</li>
                <li>Neurosurgeon-in-Chief, Duke University Hospital</li>
                <li>Program Director, Division of Neurosurgery/Department of Surgery</li>
            </ul>
                <p class="des">Allan H. Friedman, MD, is an internationally recognized tumor and vascular neurosurgeon. He has a career-long interest in neuro-oncology, is responsible for over ninety percent of all tumor resections and biopsies conducted at Duke, and has written hundreds of articles on the neurosurgical management of brain tumors and vascular lesions. He is head of the Laboratory of Neurosurgical Oncology and an Associate Chief of the Preuss Laboratory for Brain Tumor Research.
                </p>
                </div>
        </div><br>
                      <div id="tk">
            <img src="./assets/tk.png" alt="tkheadshot" class="headshot">
            <h3>Terry Kruger</h3>
            <h4>ASSOCIATE DIRECTOR</h4>
            <ul class="dlist">
                <li>University of Minnesota ’77,  Varsity Softball</li>
                <li>University of Minnesota Graduate School, MS</li>
            </ul>
                <p class="des">Terry Kruger worked in adolescent therapy, crisis intervention, and was the Maui Island Director of the Girl Scouts before she came to Duke University in 2000. She has been the Associate Director of CAPE since its inception in 2005. She is responsible for the management, growth, and success of the program over the past six years.
                </p>
                </div></div></div>
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
            <h2 class="curric">School Year Curriculum</h2>
                <h3 id="cons" @click="showCons">Consultations</h3>
                    <p v-show="consinfo" class="info">For one semester each year, students at the sophomore level and beyond shadow physicians as they perform new patient consultations at The Preston Robert Tisch Brain Tumor Center at Duke Medical Center. They learn the essentials of conducting a history and neurological examination, and very rapidly they are given primary responsibility as the first healthcare provider to see a new patient, take a history, do a neurological examination, and report to the attending physician.  
                    </p>
                <h3 id="club" @click="showClub">Journal Club</h3>
                    <p class="info" v-show="clubinfo">At the monthly journal club meetings, CAPE students discuss assigned readings which address a broad span of issues in the medical field. 
                    </p>
                <h3 id="dinner" @click="showDin">Role Model Dinner</h3>
                    <p class="info" v-show="dininfo">The CAPE students host female medical students, housestaff, attending physicians and other healthcare providers.  They are given a real-world, rigorous exposure to the path they seek to follow.
                    </p>
                <h3 id="sess" @click="showLead">Leadership Sessions</h3>
                    <p class="info" v-show="leadinfo">CAPE students meet with leaders both inside and outside of Medicine to gain understanding of the skill sets necessary to develop and provide leadership in the medical, academic and community arenas.
                    </p>
              </div>
          <div class="cs" id="cs2">
          <h2 class="curric">Summer Curriculum</h2>
                <h3 id="intern" @click="showInt">Internship</h3>
                    <ul class="list" v-show="intinfo">
                        <li class="item">Between Sophomore and Junior Year</li>
                        <li class="item">Students rotate through the  clinical practices of CAPE faculty; participate in inpatient rounding, outpatient clinics, and any didactic sessions that occur during the students' time with their respective physicians
                        </li>
                        <li class="item">Those students who have a particular interest in laboratory work and who are 
                            considering careers as physician-scientists have the opportunity to intern in the laboratories of the CAPE basic science faculty</li>
                    </ul>
                <h3 id="speak" @click="showSpeak">Speakers</h3>
                    <ul class="list" v-show="speakinfo">
                        <li class="item">Weekly speakers every Friday</li>
                        <li class="item">Discuss a wide range of topics from ethical issues to career paths and objectives</li>
                        <li class="item">Women physicians specifically discuss balancing life as a physician and how to empower other women</li>
                    </ul>
                <h3 id="teach" @click="showTeach">Teaching</h3>
                    <ul class="list" v-show="teachinfo">
                        <li class="item">CAPE Faculty teach weekly sessions</li>
                        <li class="item">Topics cover essentials of clinical medicine: history and physicals, specific diseases, symptom complexes </li>
                    </ul>
            </div>
              </div>
          </div>
              <div v-show="join">
                    <h2 id="interest">Are you interested in joining the CAPE Program?</h2>
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
          <div v-show="donate">
            <p class="b">If you would like to donate to CAPE, you can either donate online <a>here</a>, or you can print this form and fill it out as you like. All donations are much appreciated!</p>
              <div id="bigimag"><hr><br>
          <img src="./assets/Picture1.png" alt="womenandsports" id="womensports">
      </div><hr>
    
    
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
        bshow: false,
        consinfo: true,
        clubinfo: true,
        dininfo: true,
        leadinfo: true,
        intinfo: true,
        teachinfo: true,
        speakinfo: true,
    
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
            this.meetS=false;
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
            this.donate=true;
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
        },
        showCons(){
            var changed=false
            if (this.consinfo===true){
                this.consinfo=false;
                changed=true;
            }
            if (this.consinfo===false && changed===false){
                this.consinfo=true;
            }
        },
        showClub(){
            var changed=false
            if (this.clubinfo===true){
                this.clubinfo=false;
                changed=true;
            }
            if (this.clubinfo===false && changed===false){
                this.clubinfo=true;
            }
        },
        showDin(){
            var changed=false
            if (this.dininfo===true){
                this.dininfo=false;
                changed=true;
            }
            if (this.dininfo===false && changed===false){
                this.dininfo=true;
            }
        },
        showLead(){
            var changed=false
            if (this.leadinfo===true){
                this.leadinfo=false;
                changed=true;
            }
            if (this.leadinfo===false && changed===false){
                this.leadinfo=true;
            }
        },
        showInt(){
            var changed=false
            if (this.intinfo===true){
                this.intinfo=false;
                changed=true;
            }
            if (this.intinfo===false && changed===false){
                this.intinfo=true;
            }
        },
        showSpeak(){
            var changed=false
            if (this.speakinfo===true){
                this.speakinfo=false;
                changed=true;
            }
            if (this.speakinfo===false && changed===false){
                this.speakinfo=true;
            }
        },
        showTeach(){
            var changed=false
            if (this.teachinfo===true){
                this.teachinfo=false;
                changed=true;
            }
            if (this.teachinfo===false && changed===false){
                this.teachinfo=true;
            }
        },
        
    }
}
</script>

<style lang="scss">
    #bod{
        background: #fffff4;
/*        background-image: url("./assets/grey3.jpg");*/
        color: black;
        max-width: 80%;
        margin: 0 auto;
        font-family: "Helvetica"
    }
    body{
        background-color:#fffff4; 
    }
#app {
  text-align: center;
}
        header{
        max-width: 100%;
/*
        background-image: url("./assets/header.jpg");
        background-size: cover;
*/
    }

    #big{
        font-size: 45pt;
        font-family: "Helvetica";
        font-weight: 100;
        color: darkred;
        margin-top: 1%;
        margin-bottom: 1%;
    }

a {
  color: #42b983;
}
    .option{
        border: solid thin darkred;
        color: darkred;
        padding: 5px;
        display: inline-block;
        margin: 0 10px;
    }
    .option:hover{
        cursor: pointer;
        background-color: goldenrod;
    }
    #duke{
        max-width: 80%;
        border: solid medium darkred;
    }
    #logo{
        max-width: 80%;
    }
    #top{
        list-style-type: none;
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
    }
    #cape{
        width: 27%;
        
    }
    #dukie{
        width: 12%;
  
    }
    #htitle{
  
    }
    #name{
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
        border: solid thin #813F0B;
        max-width: 60%;
        margin: 0 auto;
        background-color: white;
        color: #813F0B;
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
        border: groove medium darkred;
        max-width: 40%;
        margin: 0 auto;
    }
    .others{
        max-width: 50%;
    }
    #cont{
        display: flex;
        justify-content: space-evenly;
        border: solid thin brown;
        color: saddlebrown;
        background-color: white;
    }
    #exec{
        color: darkred;
    }
    .cs{
        border: solid thin black;
        max-width: 48%;
        min-width: 48%;
        padding: 5px;
        color: aliceblue;
    }
    #cs1{
        background-color: maroon;
    }
    #cs2{
        background-color: #933a16;
    }
    .dlist{
        list-style-type: none;
        margin-right: 7%;
        font-size: 10pt;
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
        border: solid medium #420d09;
        background-color: #CC7722;
        color: wheat;
        padding: 6px;
        
    }
    #contact{
        border: solid thin #420d09;
        max-width: 40%;
        margin: 0 auto;
        color: #420d09;
    }
    .b{
        font-weight: bold;
        color: #420d09;
    }
    #interest{
        color: #420d09;
    }
    #direc{
        background-color: #D2B55B;
        padding: 0;
        margin: 0;
    }
    #btitle{
        background-color: #CEB180;
    }
    #cons{
        background-color: #CC7722;
    }
    #club{
        background-color: #CC7722;
    }
    #dinner{
        background-color: #CC7722;
    }
    #sess{
        background-color: #CC7722;
    }
    #intern{
        background-color: #C49102;
    }
    #speak{
        background-color: #C49102;
    }
    #teach{
        background-color: #C49102;
    }
    h5{
        font-size: 12pt;
    }
    #bigimag{
/*        background: linear-gradient(lightgray, dimgray);*/
    }
    #board{
        margin: 0;
    }
    #alld{
        background-color: #A5A2A0;
        margin: 0;
    }
    #d{
        background-color: #A5A2A0;
    }
    .headshot{
        max-width: 30%;
        margin: 3px;
        border: solid thin black;
    }
    #introex{
        margin: 0 auto;
        color: #420d09;
    }
    #images{
        display: flex;
        justify-content: center;
        align-items: flex-start;
    }
    .smaller{
        max-width: 30%;
        border: groove thin #420d09;;
        margin: 5px;
    }
    #readmore{
        color: #420d09;
    }
    .des{
        padding: 7px;
        font-size: 11pt;
    }
    h2{
        margin-top: 1%;
        margin-bottom: 1%;
    }
    .curric{
        text-decoration: underline;
    }
    #studpics{
        list-style-type: none;
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
    }
    #studpics li{
        width: 20%;
        border: solid thin darkblue;
    }
    #studpics li img{
        width: 100%; 
    }
    .caption{
        font-size: 10pt;
        color: darkblue;
    }
    .blue{
        font-weight: bold;
        color: darkblue;
        text-decoration: underline;
    }
    #whoare{
        font-size: 14pt;
        border: solid thin #000080;
        padding: 10px;
        color: lightblue;
        background: darkred;
    }
</style>
