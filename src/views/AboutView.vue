<template>
    <main>
      <section id="about">
        <div class="container-fluid img-fluid">
          <NavbarC/>
          <div class="row d-flex flex-column flex-md-row">
            <div loading="lazy" class="img1">
              <div class="home-text col">
                <h1 
                  id="heading-homepage"
                  style="padding-top: 15rem; font-size: 50px"
                  class="lead display-6">
                  ABOUT & TESTIMONIALS
                </h1>
              </div>
            </div>
          </div>
        </div>
      </section>
    </main>
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
    url(https://i.postimg.cc/qM0WdYMm/miguel-alcantara-lt-Be-ID9-Bw-I-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
</style>
