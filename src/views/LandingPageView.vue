<template>
  <div class="home">
    <main>
      <section id="home">
        <div class="container-fluid">
          <div class="row d-flex flex-column flex-md-row">
            <div loading="lazy" class="img1">
              <div class="home-text col">
                <h1
                  id="heading-homepage"
                  style="padding-top: 15rem; font-size: 50px"
                  class="lead display-6"
                >
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

export default {
  name: "HomeView",
  components: {
    FooterC
  },
};
</script>

<style scoped>
main {
  width: 100vw;
  height: 100vh;
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
    url(https://i.postimg.cc/Px3ypZkD/landingpage-img.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
</style>
