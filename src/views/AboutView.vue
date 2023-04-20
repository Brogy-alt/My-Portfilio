<template>
  <main>
    <NavbarC />
    <section id="about">
      <div class="container-fluid img-fluid">
        <div class="row d-flex flex-column flex-md-row">
          <div loading="lazy" class="img1">
            <div class="home-text col">
              <h1 id="heading-aboutpage" style="padding-top: 15rem; font-size: 50px" class="lead display-6">
                ABOUT & TESTIMONIALS
              </h1>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>

  <div>
  <section id="about">

    <div class="about-text-section">
      <h2 class="about-heading">About me</h2>

    </div>

    <div class="container text-center" >
      <div class="row align-items-start" >
        <div class="col">
          <img src="" alt="img">
        </div>
        <div class="col">
          <p class=" text-dark text-start">I am a 21 year old web developer who has recently completed my learning phase at
            Life Choices Academy and successfully
            completed the course and is now a full stack developer. In my spare time I produce music / make youtube
            content because my passion lies with everything revolved around music.</p>
        </div>
        <div class="col">
          <div class="row">
                    <ul class="icons" style="font-size: 30px;">
                        <li><a href=""><i id="linkedin" class="fa fa-linkedin text-dark"></i></a></li>
                        <li><a href="https://www.instagram.com/?__coig_restricted=1"><i id="ig" class="fa fa-instagram text-dark"></i></a></li>
                        <li><a href="https://www.youtube.com/"><i id="yt" class="fa fa-youtube text-dark"></i></a></li>
                        <li><a href="https://twitter.com/?lang=en-za"><i id="twitter" class="fa fa-twitter text-dark"></i></a></li>
                    </ul>
            </div>
        </div>
      </div>
    </div>
  </section>
  <FooterC />
</div>

</template>

<script>
import FooterC from '@/components/FooterC.vue'
import NavbarC from '@/components/NavbarC.vue'

export default {
  name: "HomeView",
  components: {
    FooterC,
    NavbarC
  },

};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap');

main {
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
  url(https://i.postimg.cc/qM0WdYMm/miguel-alcantara-lt-Be-ID9-Bw-I-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  /* Make the image responsive */
  height: auto;

}

h2,
h3,
h4,
h5 {
  color: black;
}

#about {
  height: 100vh;
  width: 100vw;

}

.container {
  border: 1px solid;
  padding: 10px;
  box-shadow: 5px 10px #aca7a7;
  
  
}



#heading-aboutpage {
  font-family: 'Fjalla One', sans-serif;


}

.about-heading {
  margin: auto;
  font-family: 'Fjalla One', sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 40px;
  padding-top: 2rem;
  padding-bottom: 2rem;

}



#linkedin:hover{
  transform: scale(1.1);
  transition: all ease 500ms;
}
#ig:hover{
  transform: scale(1.1);
  transition: all ease 500ms;
}
#yt:hover{
  transform: scale(1.1);
  transition: all ease 500ms;
}
#twitter:hover{
  transform: scale(1.1);
  transition: all ease 500ms;
}

/* @media (max-width: 400px) {
  .col p {
    height: 40px !important ;
   
  }
} */
</style>
