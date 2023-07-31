<template>
    <main>

        <div>
        <header>
    <div class="test">
      <nav class="navbar navbar-expand-lg sticky">
      <div class="container-fluid bg-transparent">
        <a class="navbar-brand bg-transparent text-light"  style="font-family: 'Fjalla One', sans-serif; font-size: 25px;" href="#">.PORTFOLIO</a>
        <button class="navbar-toggler text-bg-light" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse " id="navbarSupportedContent">
          <ul class="navbar-nav ms-auto mb-2 mb-lg-0" style="font-family: 'Fjalla One', sans-serif; font-size: 19px;">
            <li class="nav-item">
              <a class="nav-link active text-light" aria-current="page" href="/">HOME</a>
            </li>
            <li class="nav-item">
              <a class="nav-link active text-light" aria-current="page" href="#about-page">ABOUT</a>
            </li>
            <li class="nav-item">
              <a class="nav-link active text-light" aria-current="page" href="#resume-page">RESUME</a>
            </li>
            <li class="nav-item">
              <a class="nav-link active text-light" aria-current="page" href="#skills-page">SKILLS</a>
            </li>
            <li class="nav-item">
              <a class="nav-link active text-light" aria-current="page" href="#Contact-page">CONTACT</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    </div>
  
</header>
    </div>
    

        <section id="about">
            <div class="home">
           
      <div class="home container d-flex align-items-center justify-content-center">
        <div class="row">
            <div class="col landing-text" style="padding-top: 12rem; ">
                <h6>Welcome to my personal portfolio</h6>
                <h1 class="text-hi">Hi, I'm <span class="name">Brogan Gys</span></h1>
                <h3>A Full Stack Web Developer</h3>
            </div>
        </div>
    </div>
</div>
      </section>
    </main>

<div id="about-page">
   <AboutC/>
</div>

<div id="resume-page">
    <ResumeC/>
</div>

<div id="Skills-page">
    <SkillsC/>
</div>

<div id="Contact-page">
    <ContactC/>
</div>
  
  <FooterC />
</template>

<script>
import AboutC from '@/components/AboutC.vue';

import ResumeC from '@/components/ResumeC.vue';

import SkillsC from '@/components/SkillsC.vue';

import ContactC from '@/components/ContactC.vue';


export default {
  name: "HomeView",
  components: {
    AboutC,ResumeC,SkillsC,ContactC
  },
};
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap');

main {
  min-height: 100vh;
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
  url(https://i.postimg.cc/W4MzbZ0f/ashkan-forouzani-mb-Lr6-NEat-MI-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  height: auto;
 
}

.text-hi{
  font-size: 102px;
  font-family: 'Fjalla One', sans-serif;
  position: relative;
  text-align: center;
}

.name{
  font-family: 'Fjalla One', sans-serif;
  position: relative;
  text-align: center;
  font-size: 102px;
  /* color: rgba(255, 255, 255, 0.2); */
  /* background-image: url("https://i.postimg.cc/sXD1P0jT/armand-khoury-4c-BVro7-SHLs-unsplash.jpg"); */
  /*   background-position: center; */
  background-size: auto;
  width: 100%;
  /* background-repeat: repeat-x; */
  /* -webkit-background-clip: text; */
  /* animation: animate 10s linear infinite; */
}

@keyframes animate {
  0% {
    background-position: left 0px top 0px;
  }
  40% {
    background-position: left 800px top 0px;
  }
}

@media (max-width: 400px) {
  .landing-text span {
    font-size: 75px !important ;
   
  }

  .landing-text  {
    padding-top: 8rem !important;
  }

  .landing-text h1{
    font-size: 75px;
  }

  .landing-text h3{
    font-size: 20px;
  }

}

@media (min-width: 999px) {
  .navbar-nav {
    margin-right: 3rem;
   
  }
  .navbar-brand {
    margin-left: 3rem;
  }
}

/* ###################################################################### navbar ###################################################################### */



@import url('https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap');

  .navbar, .container-fluid {
    background-color: transparent;
    /* position: relative; */
    backdrop-filter: blur(5px);
    
  }  
  
  .navbar-toggler , .navbar-toggler-icon {
    color: #ffffff;
  };

  .navbar-toggler {
    border-color: white;
  };



</style>