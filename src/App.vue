<template>
  <div id="app">
    <AppHeader :headerMenuItems="headerMenuItems" />
    <AppMain />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
  data() {
    return {
      headerMenuItems: [
        {
          text: "Home",
          link: "#",
        },
        {
          text: "Who We Are",
          link: "#",
        },
        {
          text: "What We Do",
          link: "#",
        },
        {
          text: "Where We Work",
          link: "#",
        },
        {
          text: "Careers",
          link: "#",
          tag: "Apply",
        },
        {
          text: "News",
          link: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./style/variables.scss";
@import "./style/common.scss";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
