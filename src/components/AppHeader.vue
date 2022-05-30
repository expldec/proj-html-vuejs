<template>
  <header>
    <div class="container">
      <div class="header my-3 d-flex justify-content-between">
        <div class="header__left">
          <img
            id="header-logo"
            src="../assets/images/logo_seo_2x.png"
            alt="Avada SEO"
          />
        </div>
        <div class="header__right d-flex align-items-center">
          <ul>
            <li v-for="(item, index) in headerMenuItems" :key="index">
              <a :href="item.link" class="link-dark">{{ item.text }}</a>
              <span
                v-if="item.tag"
                class="ms-tag btn btn-sm btn-outline-primary"
                >{{ item.tag }}</span
              >
            </li>
          </ul>
          <a href="#" class="btn text-white btn-primary">Get in touch now</a>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  props: { headerMenuItems: Array },
};
</script>

<style lang="scss" scoped>
.header {
  height: 3rem;
}
#header-logo {
  height: 100%;
}
ul {
  list-style: none;
  margin-bottom: 0;
  li {
    display: inline-flex;
    align-items: center;
    margin-right: 1rem;
    font-size: 0.9rem;
    a {
      text-decoration: none;
    }
    .ms-tag {
      margin-left: 0.4rem;
      font-size: 0.8rem;
    }
  }
}
</style>
