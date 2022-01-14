<template>
  <div id="app">
    <Header />

    <main>
      <Main />

    </main>

    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer

  },
};
</script>

<style lang="scss">
@import './style/general.scss';
@import './style/variables.scss';

#app {
  font-family: "Roboto", Arial, Helvetica, sans-serif;
}

.comics {
  height: 200px;
  background-color: $dark;
}
</style>
