<template>
  <div class="skills-page">
    <!-- <main>
      <section id="skills-page">
        <div class="container-fluid">
        
          <div class="row d-flex flex-column flex-md-row">
            <div loading="lazy" class="img1 img-fluid">
              <div class="home-text col">
                <h1
                  id="heading-skillspage"
                  style="padding-top: 20rem; font-size: 50px"
                  class="lead display-6"
                >
                  SKILLS AND PROJECTS
                </h1>
              </div>
            </div>
          </div>
        </div>
      </section>
    </main> -->

    <div class="skills-section">
      <div class="skills-header">
        <h2 class="skills-heading text-dark">SKILLS</h2>
      </div>
      <div class="skills-container" style="padding-top: 5rem">
        <div class="skills-box">
          <div class="skills-title">
            <div class="skills-img">
              <img
                src="https://i.postimg.cc/vB9bnM6B/html-img.png"
                alt=""
                class="skills-icons"
              />
            </div>
            <h3>HTML 5</h3>
          </div>
        </div>

        <div class="skills-box">
          <div class="skills-title">
            <div class="skills-img">
              <img
                src="https://i.postimg.cc/QMG6t3sS/css-icon.png"
                alt=""
                class="skills-icons"
              />
            </div>
            <h3>CSS</h3>
          </div>
        </div>

        <div class="skills-box">
          <div class="skills-title">
            <div class="skills-img">
              <img
                src="https://i.postimg.cc/MGpDPb02/javascript-icon.png"
                alt=""
                class="skills-icons"
              />
            </div>
            <h3>JAVASCRIPT</h3>
          </div>
        </div>

        <div class="skills-box">
          <div class="skills-title">
            <div class="skills-img">
              <img
                src="https://i.postimg.cc/xTQLp3Yx/nodejs-icon.png"
                alt=""
                class="skills-icons"
              />
            </div>
            <h3>NODE.JS</h3>
          </div>
        </div>

        <div class="skills-box">
          <div class="skills-title">
            <div class="skills-img">
              <img
                src="https://i.postimg.cc/BnBgqwZ1/mysql-icon.png"
                alt=""
                class="skills-icons"
              />
            </div>
            <h3>MSQL</h3>
          </div>
        </div>

        <div class="skills-box">
          <div class="skills-title">
            <div class="skills-img">
              <img
                src="https://i.postimg.cc/g2gSWkKZ/icons8-bootstrap-512.png"
                alt=""
                class="skills-icons"
              />
            </div>
            <h3>BOOSTRAP</h3>
          </div>
        </div>

        <div class="skills-box">
          <div class="skills-title">
            <div class="skills-img">
              <img
                src="https://i.postimg.cc/P5dDMWYW/Ui-ux-icon.png"
                alt=""
                class="skills-icons"
              />
            </div>
            <h3>UI/UX</h3>
          </div>
        </div>

        <div class="skills-box">
          <div class="skills-title">
            <div class="skills-img">
              <img
                src="https://i.postimg.cc/V604cq7S/wordpress-icon.png"
                alt=""
                class="skills-icons"
              />
            </div>
            <h3>WORDPRESS</h3>
          </div>
        </div>

        <div class="skills-box">
          <div class="skills-title">
            <div class="skills-img">
              <img
                src="https://i.postimg.cc/ZRT9Z4Y1/icons8-vue-js-480.png"
                alt=""
                class="skills-icons"
              />
            </div>
            <h3>VUE.JS</h3>
          </div>
        </div>

        <div class="skills-box">
          <div class="skills-title">
            <div class="skills-img">
              <img
                src="https://i.postimg.cc/NjZSddtT/icons8-seo-64.png"
                alt=""
                class="skills-icons"
              />
            </div>
            <h3>SEO</h3>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- <section id="project-page">
    <div class="container-fluid">
      <div class="row d-flex flex-column flex-md-row">
        <div loading="lazy" class="img1 img-fluid">
          <div class="home-text col">
            <h1
              id="heading-projectpage"
              style="padding-top: 20rem; font-size: 50px"
              class="lead display-6"
            >
              PROJECTS
            </h1>
          </div>
        </div>
      </div>
    </div>
  </section> -->

  <!-- Projects Section -->
  <div class="projects-section">
    <div class="projects-header">
      <h2 class="projects-heading text-dark">PROJECTS</h2>
    </div>

    <div class="scroll-container">
    <div class="project-container p-0 py-5">
      <div class="container">
        <div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-4">
          <div v-for="project in projects" :key="project.id" class="col">
            <div class="card">
              <img
                :src="project.image"
                class="card-img-top"
                :alt="project.title + ' project'"
                style="height: 200px; object-fit: cover"
              />
              <div class="card-body">
                <h5 class="card-title">{{ project.title }}</h5>
              </div>
              <div class="card-footer d-flex justify-content-center">
                <div class="text-light">
                  <a
                 target="_blank"  :href="project.link"
                    class="linktr__goal r-link" style="font-size: 17px;"
                    
                    >View</a
                  >

                
                </div>
                
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  </div>
</template>

<script>
export default {
  name: "HomeView",
  data() {
    return {
      projects: [
        {
          id: 1,
          title: "The KitCollective (WordPress)",
          image:
            "https://i.postimg.cc/HLZrBdLt/The-kit-collective-duo-word-press-project.png",
          link: "https://dev-thekitcollective.pantheonsite.io/",
        },
        {
          id: 2,
          title: "My Webstore (WordPress)",
          image:
            "https://i.postimg.cc/8P6NHzN7/Screenshot-2023-07-12-123409.png",
          link: "https://dev-prodbrogy-store.pantheonsite.io/",
        },
        {
          id: 3,
          title: "Cut Connect (WordPress)",
          image: "https://i.postimg.cc/brstQrb3/Screenshot-2023-09-13-091217.png",
          link: "hhttps://dev-cut-connect.pantheonsite.io/",
        },
        {
          id: 6,
          title: "4di Website (Client work WORDPRESS)",
          image:
            "https://i.postimg.cc/hGpJB03G/4DI.png",
          link: "https://4diteam.lcstudio-incubate.co.za/",
        },
        {
          id: 4,
          title: "Country Stats (JavaScript API)",
          image:
            "https://i.postimg.cc/SNZq0YVB/Screenshot-2023-09-07-121003.png",
          link: "https://country-stats-project.netlify.app/",
        },
        {
          id: 5,
          title: "Login In & Out System (PHP)",
          image:
            "https://i.postimg.cc/Z5D7gwhF/Screenshot-2023-08-17-085240.png",
          link: "https://php-project2810.000webhostapp.com/",
        }
      ],
    };
  },
};
</script>

<style scoped>
main {
  min-height: 100vh;
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
    url(https://i.postimg.cc/Tw99zpwZ/indivar-kaushik-gc-A0-W3-OOOts-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
}

h1,h2,h3{
  font-family: "Fjalla One", sans-serif;
}

p , a{
  font-size: 19px;
  font-family: "Rubik", sans-serif;
  
}

#heading-skillspage {
  font-family: "Fjalla One", sans-serif;
}

.skills-section {
  padding-top: 20px;
  min-height: 100vh;
  width: 100%;
}

.skills-header {
  text-align: center;
  color: #fff;
  padding: 1rem;
  position: relative;
}

.skills-header:after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 100px;
  height: 4px;
  background-color: #1D1D1D;
  border-radius: 2px;
}

.skills-container {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  justify-content: center;
  align-items: center;
  text-align: center;
  grid-gap: 1rem;
  padding: 1rem 80px;
  font-size: 1.2rem;
}

.project-container {
  display: flex;
  justify-content: center;
  margin: auto;
  text-align: center;
  grid-gap: 1rem;
  font-size: 1.2rem;
}

.skills-box {
  padding: 1rem;
  color: #000;
  cursor: pointer;
}

.skills-box:hover > .skills-title:after,
.skills-box:hover > .skills-title:before {
  width: 30px;
}

.skills-box:hover .skills-img {
  transform: translateX(-20px);
}

.skills-title {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0.5rem;
  margin-bottom: 0.5rem;
  position: relative;
}

.skills-title:after {
  content: "";
  position: absolute;
  bottom: 0;
  right: 50%;
  width: 20px;
  height: 4px;
  border-radius: 2px 0 0 2px;
  background-color: #1D1D1D;
  transition: 0.5s;
}

.skills-title:before {
  content: "";
  position: absolute;
  bottom: 0;
  left: 50%;
  width: 100px;
  height: 4px;
  border-radius: 0 2px 2px 0;
  background-color: #1D1D1D;
}

.skills-icons {
  width: 50px;
  z-index: 2;
}

.skills-img {
  width: 100px;
  height: 100px;
  position: relative;
  border-radius: 45px;
  background-color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: 0.5s;
}

.skills-img:after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 50%;
  height: 90px;
  /* background: rgba(100, 100, 100, 0.5); */
  border-radius: 45px 0 0 45px;
}
.skills-title h3 {
  color: #333;
  margin-top: 0.5rem;
}
@media screen and (max-width: 990px) {
  .skills-container,
  .project-container {
    grid-template-columns: repeat(2, 1fr);
    padding: 2rem 50px;
  }
}

@media screen and (max-width: 650px) {
  .skills-container {
    grid-template-columns: 2fr;
    padding: 2rem 50px;
  }
}

.card-body {
  padding: 0 !important;
}



button:disabled {
  pointer-events: none;
}

button:hover {
  color: #fff;
  background-color: #1a1a1a;
  box-shadow: rgba(0, 0, 0, 0.25) 0 8px 15px;
  transform: translateY(-2px);
}

button:active {
  box-shadow: none;
  transform: translateY(0);
}

/* Convert project images to grayscale by default */
.card-img-top {
    filter: grayscale(100%);
    transition: filter 0.3s ease;
  }

  /* Restore the original color when hovered over */
  .card:hover .card-img-top {
    filter: grayscale(0%);
  }

/* ###############################################SKILLS################################################ */

#project-page {
  min-height: 100vh;
  background: linear-gradient(rgba(255, 255, 255, 0.035), rgba(0, 0, 0, 1)),
    url(https://i.postimg.cc/tgmxQsZc/hal-gatewood-t-Zc3vj-PCk-Q-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
}



.projects-header {
  text-align: center;
  color: #fff;
  padding: 1rem;
  position: relative;
}

.projects-header:after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 100px;
  height: 4px;
  background-color: #1D1D1D;
  border-radius: 2px;
}

#heading-projectpage {
  font-family: "Fjalla One", sans-serif;
}

/* Custom CSS for equal-sized cards */
.project-container .card {
  min-height: 100%;
}

/* Optionally, you can add custom CSS for equalizing card titles if needed */
.card-title {
  min-height: 2.8rem;
}

.linktr__goal{
  background-color: #1D1D1D;
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


</style>
