<template>
  <div id="app">
    <AppHeader :navMenuItems="navMenuItems" />
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
      navMenuItems: [
        {
          text: "Home",
          link: "#",
          isActive: true,
          isButton: false,
        },
        {
          text: "Who We Are",
          link: "#",
          isActive: false,
          isButton: false,
        },
        {
          text: "What We Do",
          link: "#",
          isActive: false,
          isButton: false,
        },
        {
          text: "Where We Work",
          link: "#",
          isActive: false,
          isButton: false,
        },
        {
          text: "Careers",
          link: "#",
          tag: "Apply",
          isActive: false,
          isButton: false,
        },
        {
          text: "News",
          link: "#",
          isActive: false,
          isButton: false,
        },
        {
          text: "Get in touch now",
          link: "#",
          isActive: false,
          isButton: true,
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./style/variables.scss";
@import "./style/common.scss";
@import "~@fortawesome/fontawesome-free/css/all.min.css";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
