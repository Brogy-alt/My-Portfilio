<template>
    <main>
      <MenuC />
      <section id="about">
        <div class="home">
      <div class="home container d-flex align-items-center justify-content-center">
        <div class="row">
            <div class="col landing-text" style="padding-top: 12rem; ">
                <h6>Welcome to my personal portfolio</h6>
                <h1 class="text-hi">Hi, I'm <span>Brogan Gys</span></h1>
                <h3>A Full Stack Software Developer</h3>
            </div>
        </div>
    </div>
</div>
      </section>
    </main>
  
  <FooterC />
</template>

<script>
// import MenuC from "@/components/MenuC.vue";

// export default {
//   name: "HomeView",
//   components: {
//     MenuC,
//   },
// };
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

span{
  font-family: 'Fjalla One', sans-serif;
  position: relative;
  text-align: center;
  font-size: 102px;
  color: rgba(255, 255, 255, 0.2);
  background-image: url("https://i.postimg.cc/sXD1P0jT/armand-khoury-4c-BVro7-SHLs-unsplash.jpg");
  /*   background-position: center; */
  background-size: auto;
  width: 100%;
  background-repeat: repeat-x;
  -webkit-background-clip: text;
  animation: animate 10s linear infinite;
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






</style>