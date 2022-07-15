<template>
  <div id="app">
    <HeaderContainer />
    <Main />
    <Footer />
  </div>
</template>

<script>
import HeaderContainer from "./components/HeaderContainer.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    HeaderContainer,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Yanone+Kaffeesatz:wght@500&display=swap');
@import "~bootstrap/scss/bootstrap.scss";
@import "./style/variables.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body {
  font-family: 'Yanone Kaffeesatz', sans-serif;
}
</style>
