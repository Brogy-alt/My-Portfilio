<template>
  <main>
    <div>
      <header>
        <div class="test">
          <nav class="navbar navbar-expand-lg sticky mx-auto">
            <div class="container-fluid ">
              <a
                class="navbar-brand bg-transparent text-light "
                style="font-family: 'Fjalla One', sans-serif; font-size: 25px"
                href="#"
                >.PORTFOLIO</a
              >
              <button
                class="navbar-toggler text-bg-light"
                type="button"
                data-bs-toggle="collapse"
                data-bs-target="#navbarSupportedContent"
                aria-controls="navbarSupportedContent"
                aria-expanded="false"
                aria-label="Toggle navigation"
              >
                <span class="navbar-toggler-icon"></span>
              </button>
              <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul
                  class="navbar-nav ms-auto mb-2 mb-lg-0"
                  style="font-family: 'Fjalla One', sans-serif; font-size: 19px"
                >
                  <li class="nav-item">
                    <a
                      class="nav-link active text-light"
                      aria-current="page"
                      href="/"
                      >HOME</a
                    >
                  </li>
                  <li class="nav-item">
                    <a
                      class="nav-link active text-light"
                      aria-current="page"
                      href="#about-page"
                      >ABOUT</a
                    >
                  </li>
                  <li class="nav-item">
                    <a
                      class="nav-link active text-light"
                      aria-current="page"
                      href="#resume-page"
                      >RESUME</a
                    >
                  </li>
                  <li class="nav-item">
                    <a
                      class="nav-link active text-light"
                      aria-current="page"
                      href="#skills-page"
                      >SKILLS</a
                    >
                  </li>
                  <li class="nav-item">
                    <a
                      class="nav-link active text-light"
                      aria-current="page"
                      href="#Contact-page"
                      >CONTACT</a
                    >
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
        <div
          class="home container d-flex align-items-center justify-content-center"
        >
          <div class="row">
            <div class="col landing-text">
              <h6>Welcome to my personal portfolio</h6>
              <h1 class="text-hi">
                Hi, I'm <span class="name">Brogan Gys</span>
              </h1>
              <h3>A Front-End Web Developer</h3>
              <div class="CV">
                <a style="font-size: 15px;"
                  href="https://drive.google.com/file/d/1jbUa7JOE4y6Q2AVwFO4jg4zyRywORGjX/view?usp=sharing"
                  class="linktr__goal r-link"
                  target="_blank"
                  >Download My CV</a
                >

                <!-- <button id="download-btn"  @click="DownloadCV ">Download My CV</button> -->
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>

  <div id="about-page">
    <AboutC />
  </div>

  <div id="resume-page">
    <ResumeC />
  </div>

  <div id="Skills-page">
    <SkillsC />
  </div>

  <div id="Contact-page">
    <ContactC />
  </div>

  <FooterC />
</template>

<script>
import AboutC from "@/components/AboutC.vue";

import ResumeC from "@/components/ResumeC.vue";

import SkillsC from "@/components/SkillsC.vue";

import ContactC from "@/components/ContactC.vue";

export default {
  name: "HomeView",
  components: {
    AboutC,
    ResumeC,
    SkillsC,
    ContactC,
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap");

main {
  min-height: 100vh;
  background: 
  url(https://i.postimg.cc/qRgQM2MY/Group-2-1.png);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  height: auto;
 
}

.text-hi {
  font-size: 102px;
  font-family: "Fjalla One", sans-serif;
  position: relative;
  text-align: center;
}

.name {
  font-family: "Fjalla One", sans-serif;
  position: relative;
  text-align: center;
  font-size: 102px;
  background-size: auto;
  width: 100%;

}
a.linktr__goal.r-link{
  color: black !important;

}

.linktr__goal{
  background-color: #ffffff;
  color: rgb(8, 49, 112);
  box-shadow: rgb(8 49 112 / 24%) 0px 2px 8px 0px;
  border-radius: 2rem;
  padding: .75rem 1.5rem;
  margin: auto;
}

.r-link{
    --uirLinkDisplay: var(--rLinkDisplay, inline-flex);
    --uirLinkTextColor: var(--rLinkTextColor);
    --uirLinkTextDecoration: var(--rLinkTextDecoration, none);

    display: var(--uirLinkDisplay) !important;
    color: var(--uirLinkTextColor) !important;
    text-decoration: var(--uirLinkTextDecoration) !important;
}


@keyframes animate {
  0% {
    background-position: left 0px top 0px;
  }
  40% {
    background-position: left 800px top 0px;
  }
}

/* Styles for screens up to 300px */
@media (max-width: 300px) {
  .landing-text span {
    font-size: 40px !important;
  }

  .landing-text {
    padding-top: 8rem !important;
  }

  .landing-text h1 {
    font-size: 40px;
  }

  .landing-text h3 {
    font-size: 12px;
  }

  a.linktr__goal.r-link{
  font-size: 10px !important;

  }
}

/* Styles for screens between 301px and 500px */
@media (min-width: 301px) and (max-width: 500px) {
  .landing-text span {
    font-size: 50px !important;
  }

  .landing-text {
    padding-top: 8rem !important;
  
  }

  .landing-text h1 {
    font-size: 50px;
  }

  .landing-text h3 {
    font-size: 14px;
  }

  
  a.linktr__goal.r-link{
  font-size: 12px !important;

  }
}

/* Styles for screens between 501px and 600px */
@media (min-width: 501px) and (max-width: 600px) {
  .landing-text span {
    font-size: 60px !important;
  }

  .landing-text {
    padding-top: 6rem !important;
  }

  .landing-text h1 {
    font-size: 60px;
  }

  .landing-text h3 {
    font-size: 16px;
  }
}

/* Add more media queries for larger screen sizes if needed */

@media (min-width: 601px) and (max-width: 800px) {
  /* Styles for screens between 601px and 800px */
  .landing-text span {
    font-size: 70px !important;
  }

  .landing-text {
    padding-top: 8rem !important;
  }

  .landing-text h1 {
    font-size: 70px;
  }

  .landing-text h3 {
    font-size: 18px;
  }
}
@media (min-width: 801px) and (max-width: 900px) {
  /* Styles for screens between 601px and 800px */
  .landing-text span {
    font-size: 80px !important;
  }

  .landing-text {
    padding-top: 8rem !important;
  }

  .landing-text h1 {
    font-size: 80px;
  }

  .landing-text h3 {
    font-size: 22px;
  }
}

@media (min-width: 901px) and (max-width: 1500px) {

  .landing-text span {
    font-size: 85px !important;
  }

  .landing-text {
    padding-top: 8rem !important;
  }

  .landing-text h1 {
    font-size: 85px;
  }

  .landing-text h3 {
    font-size: 27px;
  }
}


/* Continue to add more media queries for larger screen sizes as necessary */

/* Default styles for screens larger than 1500px (no media query needed) */


@media (min-width: 999px) {
  .navbar-nav {
    margin-right: 3rem;
  }
  .navbar-brand {
    margin-left: 3rem;
  }
}





/* ###################################################################### navbar ###################################################################### */

@import url("https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap");

.navbar,


.navbar-toggler,
.navbar-toggler-icon {
  color: #ffffff;
}

.navbar-toggler {
  border-color: white;
}
</style>
