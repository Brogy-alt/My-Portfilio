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


main {
  min-height: 100vh;
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
  url(https://i.postimg.cc/W4MzbZ0f/ashkan-forouzani-mb-Lr6-NEat-MI-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  height: auto;
 
}


</style>