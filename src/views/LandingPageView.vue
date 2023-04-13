<template>
  <div class="home">
    <main>
      <section id="home">
        <div class="container-fluid ">
          <NavbarC/>
          <div class="row d-flex flex-column flex-md-row">
            <div loading="lazy" class="img1 img-fluid">
              <div class="home-text col">
                <h1 
                  id="heading-homepage"
                  style="padding-top: 15rem; font-size: 50px"
                  class="lead display-6">
                  TEXT OVER HERE
                </h1>
              </div>
            </div>
          </div>
        </div>
      </section>
    </main>
  </div>
  <FooterC />

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
main {
  width: 100vw;
  height: 100vh;
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
    url(https://i.postimg.cc/G9wyZG1N/ashkan-forouzani-mb-Lr6-NEat-MI-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
</style>
