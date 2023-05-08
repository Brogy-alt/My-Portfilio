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
                    id="heading-skillspage"
                    style="padding-top: 15rem; font-size: 50px"
                    class="lead display-6">
                    SKILLS AND PROJECTS
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
    methods: {
    downloadCV() {
      const link = document.createElement('a');
      link.href = 'https://drive.google.com/file/d/1ZSx5pq4RdCV0U6Y_g6PTe57TmXQjEE7i/view?usp=sharing'; // Replace 'path_to_your_cv_file.pdf' with the actual path to your CV file
      link.download = 'BroganGys-CV.pdf'; // Replace 'your_cv_file_name.pdf' with the desired name for the downloaded file
      link.click();
    }
  }
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

 

  #heading-skillspage {
  font-family: 'Fjalla One', sans-serif;
}



  </style>
  