<template>
  <header>
    <div class="container">
      <div class="header my-3 d-flex justify-content-between">
        <div class="header__left">
          <img
            id="header-logo"
            src="../assets/images/logo_seo_w_2x.png"
            alt="Avada SEO"
          />
        </div>
        <div class="header__right d-flex align-items-center">
          <ul>
            <li
              v-for="(item, index) in navMenuItems"
              :key="index"
              class="ms-3 ms-xl-4"
            >
              <a
                :href="item.link"
                :class="{
                  'link-primary': item.isActive,
                  'link-light': !item.isActive,
                  'btn text-white btn-primary': item.isButton,
                }"
                >{{ item.text }}</a
              >
              <span
                v-if="item.tag"
                class="ms-tag btn btn-sm btn-outline-primary"
                >{{ item.tag }}</span
              >
            </li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  props: { navMenuItems: Array },
};
</script>

<style lang="scss" scoped>
header {
  position: absolute;
  width: 100%;
}
.header {
  height: 3rem;
  &__left {
    min-width: 180px;
    flex-basis: 180px;
  }
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
