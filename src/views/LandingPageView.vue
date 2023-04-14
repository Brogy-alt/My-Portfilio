<template>
  <div class="home">
    <main>
      <section id="home">
        <div class="container-fluid">
          <NavbarC />
          <div
            loading="lazy"
            class="img1 img-fluid"
            style="padding-top: 16rem; font-size: 50px"> 
            
            <div class="container-fluid col-sm-12">
              <h1 id="heading-homepage">Brogan Gys</h1>
            </div>
          </div>
        </div>
      </section>
    </main>
  </div>
  <FooterC />
</template>

<script>
import FooterC from "@/components/FooterC.vue";
import NavbarC from "@/components/NavbarC.vue";

export default {
  name: "HomeView",
  components: {
    FooterC,
    NavbarC,
  },
};
</script>

<style scoped>


main {
  min-height: 100vh;
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
    url(https://i.postimg.cc/G9wyZG1N/ashkan-forouzani-mb-Lr6-NEat-MI-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}



h1 {
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

/* .text-container {
  margin-top: 17%;
  text-align: center;
} */


</style>
