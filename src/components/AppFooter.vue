<template>
  <footer>
    <div class="container text-center">
      <div class="row justify-content-center">
        <div class="col-6">
          <img class="footer__logo" src="../assets/images/logo_seo_2x.png" />
        </div>
      </div>
      <div class="row">
        <div class="col-12">
          <ul class="py-5">
            <li
              v-for="(item, index) in navMenuItems"
              :key="index"
              class="mx-3 ms-xl-4"
            >
              <a
                :href="item.link"
                :class="{
                  'link-primary': item.isActive,
                  'link-dark': !item.isActive,
                }"
                >{{ item.text }}</a
              >
            </li>
          </ul>
        </div>
      </div>
      <div class="row">
        <p id="footer__credits" class="text-muted">
          Ripped by
          <a
            href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
            target="_blank"
            rel="noreferrer"
            >Morgan</a
          >
          &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;from
          <a href="https://avada.theme-fusion.com/seo/">Avada Theme</a
          >&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;No Rights
          Reserved&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;Powered by
          <a href="http://vuejs.org" target="_blank">Vue.js</a>
        </p>
      </div>
      <div class="row">
        <p class="social-links text-muted">
          <i class="fab fa-facebook"></i>
          <i class="fab fa-instagram"></i>
          <i class="fab fa-twitter"></i>
          <i class="fab fa-youtube"></i>
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
  props: { navMenuItems: Array },
};
</script>

<style lang="scss" scoped>
footer {
  padding: 4rem 0;
  .footer__logo {
    width: 150px;
  }
}
ul {
  list-style: none;
  margin-bottom: 0;
  li {
    display: inline-block;
    font-size: 0.9rem;
    a {
      text-decoration: none;
    }
  }
}
#footer__credits {
  font-size: 0.8rem;
}
.social-links i {
  margin: 0 0.5rem;
}
</style>
