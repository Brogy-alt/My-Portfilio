<template>
 <router-view/>
 <FooterC/>
</template>

<script>
  import FooterC from './components/FooterC.vue';
  export default {
    components: {
      FooterC
    }
  }
</script>

<style>

*,
*::after,
*::before {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    word-wrap: break-word;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  overflow-x: hidden
}

/* Hide both vertical and horizontal scroll bars */
body::-webkit-scrollbar {
  display: none; /* Hide scrollbar for webkit (Chrome, Safari) */
}

/* Hide scrollbar for Firefox */
body {
  scrollbar-width: none;
}

.test {
  z-index: 1;background-color: transparent;
  position: relative;
}
nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}


</style>
