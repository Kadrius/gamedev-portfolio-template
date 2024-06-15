<template>
  <div style="margin-bottom: 40px;">
    <h1>Hello!</h1>

    <div class="paragraph">
      <div>
        I'm <strong>Adrián Blanco Costas</strong>, an XR Developer with 6+ years of experience. I graduated in 2016 in Computer Engineering in the University of A Coruña and specialized in the computing area.<br/>
        I enjoy math, specially linear algebra and I thrive when using it to solve complex problems. I'm also an enthusiast on computer vision, computer graphics and functional programming.<br/><br/>
        In general, I love learning new stuff and trying new technologies. I'm always searching for new ways to improve my expertise and to apply my knowledge on XR and videogames development.
      </div>

      <!-- div style="margin-top: 20px;">I've worked on  <router-link to="/game-projects">stuff</router-link>, on <router-link to="/other-projects">other stuff</router-link>, and took part in <router-link to="/resume">a few things</router-link> as well.</div-->
      <div style="margin-top: 20px;">I'm currently working as a Senior XR Developer at Xoia Extending Reality. You can reach me at <a href="mailto:adriblanc92@gmail.com">adriblanc92@gmail.com</a> or <router-link to="/contact">through here</router-link>.</div>
    </div>

    <div class="photo">
      <img :src="`/img/Yo5-CircleMask.png`" alt="Avatar of Kadrius" /> 
    </div>

    <div style="clear:both"></div>

  </div>
</template>

<style scoped>
.paragraph {
  max-width: 750px;
  margin-bottom: 20px;
  font-size: 90%;
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
    padding: 10px;
    padding-left: 80px;
  }
}

</style>