<template>
  <div id="app">
    <Header />

    <main>
      

      <Icons />
    </main>

    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Icons from "./components/Icons.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Icons,
    Footer
  },
};
</script>

<style lang="scss">
@import './style/general.scss';

.comics {
  height: 200px;
  background-color: black;
}
</style>
