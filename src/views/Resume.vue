<template>
  <div>
    <h1>Resume</h1>

    <div class="paragraph">
      I'm <strong>Adrián Blanco</strong>, a senior XR Developer with 6+ years of experience, mainly in Unity but I have touched also Unreal.
      <br />After graduating in Computer Science from University of A Coruña, I used Unity as a hobbyist working on personal projects and doing game jams. 
      <br />I was hired soon after as a full-stack developer but I left soon because my passion was working with Unity and 3D engines development.
      <br />I joined my next company, Xoia Extending Reality, and I quickly adapted to my new role working on some prototypes at first then doing bigger and bigger projects and now, after 6 years I'm currently the Development Team Manager.
      <br />I consider myself a good communicator and thrive in multidisciplinar teams. I have experience working with technologies outside of Unity (CMS, IOT, .NET) integrating them or using them to develop services to solve concrete problems.
      <br />
      <br />Besides my professional experience, I'm passionate about technology and I love trying out new things and keeping up to date trying out the latest technologies and reading research papers related to my profesional field.
      <br />
      <br />Feel free to 
      <router-link to="/contact">contact me</router-link>.
      <br />

      <div style="margin-top:20px; margin-bottom:20px;">
        <a class="download-link" href="d/AdrianBlancoResume2024.pdf" target="_blank"><i class="fa fa-download fa-lg fa-fw"></i> Download my resume as PDF 🇪🇸 </a>        
        <div style="clear:both"></div>
      </div>
    </div>
    <div class="photo">
      <img :src="`/img/Yo2-CircleMask.png`" alt="Photo of Adrián" />
    </div>

    <div style="clear:both"></div>

    <div class="full-content">
      <h2>Work experience</h2>

      <h3>Development Team Manager - Xoia Extending Reality</h3>
      <h4>2024-Currently</h4>

      <div>
         - Technical decision making.<br />         
         - Go to person for system administration problems.<br />
         - New Employee mentor<br />
         - Develoment team manager.<br /> 
      </div>

      <div class="tech-stack">Jira Software, SCRUM, AWS (EC2, Route 53, S3)</div>

      <h3>Unity Developer - Xoia Extending Reality</h3>
      <h4>2018-Currently</h4>

      <div>
         - XR Developer using Unity3D (Windows and MacOS).<br />
         - Analyst and Senior Developer.<br />
         - Project Management.<br />
         - Deployment for several platforms (WebGL, iOS, Android, Quest2, Quest3, Windows).<br />
         - CMS development and deployment (Strapi).<br />
      </div>

      <div class="tech-stack">Unity3D, Strapi, XCode, C#, NGINX, .NET, SOLID, Git</div>

      <h3>Fullstack developer - Aldaba</h3>
      <h4>2017-2018</h4>

      <div>
        - .NET developer (Winforms).<br />
        - Backend developer (PLSQL).
      </div>

      <div class="tech-stack">.NET, C#, PLSQL</div>

      <h2>Skills</h2>

      <div class="skill-set">
        <h3>Hard</h3>
        <SkillRate name="Unity3D" :rate="4" />
        <SkillRate name="C#" :rate="4" />
        <SkillRate name="SW Design Patterns" :rate="4" />
        <SkillRate name=".NET" :rate="3" />      
        <SkillRate name="C++" :rate="3" />   
        <SkillRate name="Python" :rate="2" />   
        <SkillRate name="Shaders" :rate="1" />  
        <SkillRate name="Unreal Engine" :rate="1" />
     
      </div>

      <div class="skill-set">
        <h3>Soft</h3>
        <SkillRate name="Communication" :rate="4" />
        <SkillRate name="Adaptability" :rate="4" />
        <SkillRate name="Analitycal thinking" :rate="4" />
        <SkillRate name="Problem solving" :rate="4" />
        <SkillRate name="Project Management" :rate="3" />
        <SkillRate name="Team Management" :rate="2" /> 
      </div>
      <div style="clear:both" />

      <h2>Education</h2>

      <h3>Computer Engineering / 2010 - 2016</h3>
      <h4>Computer Engineering degree from University of A Coruña, computing area specialization</h4>
      <div>Average grade 7</div>

      <h3>Master of Science in Computer Science / 2015 - 2016</h3>
      <h4>Coursed Masters clases during erasmus year. Course taken entirely in english.</h4>

      <h2>Languages</h2>

      <h3>Spanish</h3>
      <div>Native</div>

      <h3>Galician</h3>
      <div>Native</div>

      <h3>English</h3>
      <div>C1</div>

      <h3>French</h3>
      <div>B1</div>


      <!-- <h2>Besides...</h2>
      <div>
        <h3>I ❤️ Violence</h3>
        <div>I find it really soothing to just shoot at bad guys</div>

        <h3>I 🧡 Sports</h3>
        <div>I used to be thin but then I ingested 10 kilos of steroids and proteins a day while doing 1000 push-ups.</div>

        <h3>I 💛 Politics</h3>
        <div>I hope I can have a career here someday but I might have temper issues.</div>

        <h3>I 💚 Flowers</h3>
        <div>Especially the big ones, with the trunk and leaves.</div>

      </div> -->
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import SkillRate from "@/components/SkillRate.vue";


export default defineComponent({
  name: "Resume",
  components: {
    SkillRate,
  },
});
</script>

<style scoped>
h2 {
  font-weight: 100;
  font-size: 2em;
  margin: 0px;
  padding: 0px;
  padding-top: 50px;
}
h3 {
  font-weight: 100;
  font-size: 1.6em;
  margin: 0px;
  padding: 0px;
  padding-top: 30px;
}
h4 {
  font-weight: 100;
  font-size: 1.3em;
  margin: 0px;
  padding: 0px;
  padding-top: 15px;
  font-style: italic;
}

.paragraph {
  max-width: 750px;
  margin-bottom: 20px;
  font-size: 90%;
}

.download-link {
  float:left;
  margin-right: 50px;
}

.full-content div {
  max-width: 800px;
}

.skill-set h3 {
  padding-bottom: 10px;
}

.photo img {
  height: 300px;
  width: 300px;
}

.tech-stack {
  font-style: italic;
}

.photo {
  margin-top: 50px;
  text-align: center;
}

@media only screen and (min-width: 620px){
  .paragraph {
    float: left;
  }

  .photo {
    float: left;
    padding: 30px;
    padding-left: 80px;
  }

  .skill-set {
    float: left;
    padding-right: 60px; 
  }
}
</style>