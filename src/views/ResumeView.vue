<template>
    <div class="skills-page">
      <main>
        <section id="skills-page">
          <div class="container-fluid ">
            <NavbarC/>
            <div class="row d-flex flex-column flex-md-row">
              <div loading="lazy" class="img1 img-fluid">
                <div class="home-text col">
                  <h1 
                    id="heading-homepage"
                    style="padding-top: 15rem; font-size: 50px"
                    class="lead display-6">
                    SKILLS & PROJECTS
                  </h1>
                </div>
              </div>
            </div>
          </div>
        </section>
     
      </main>


      
    </div>
  
  
  </template>
  
  <script>

  import NavbarC from '@/components/NavbarC.vue'
  
  export default {
    name: "HomeView",
    components: {

      NavbarC
    },
  };
  </script>
  
  <style scoped>
  main {
    width: 100vw;
    height: 100vh;
    background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
      url(https://i.postimg.cc/L47wJXTb/jared-brashier-6-WPcf5-D1-Xd-A-unsplash.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    border-radius: 1%;
  }
  </style>
  