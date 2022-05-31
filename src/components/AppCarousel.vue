<template>
  <div class="carousel">
    <div
      v-for="(item, index) in slides"
      :key="index"
      class="slide"
      :class="{ active: index === activeSlide }"
    >
      <div class="slide__thumbnail">
        <img :src="require(`../assets/images/${item.img}`)" alt="" />
      </div>
      <div class="slide__text mb-2">
        <div class="slide__quote mb-2">
          {{ item.quote }}
        </div>
        <div class="slide__name">
          <strong>{{ item.name }}</strong
          >, {{ item.org }}
        </div>
      </div>
    </div>
    <div class="carousel__nav">
      <div
        v-for="(item, index) in slides"
        :key="index"
        class="carousel__indicator"
        :class="{ active: index === activeSlide }"
        @click="switchActiveSlide(index)"
      ></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppCarousel",
  props: { slides: Array },
  data: function () {
    return {
      activeSlide: 0,
    };
  },
  methods: {
    switchActiveSlide(index) {
      this.activeSlide = index;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.carousel {
  position: relative;
}
.slide {
  position: absolute;
  top: 0;
  left: 0;
  opacity: 0;
  z-index: -10;
  &.active {
    transition: opacity ease-in-out 0.5s;
    position: relative;
    opacity: 1;
    z-index: 0;
  }
  &__thumbnail {
    max-width: 10rem;
    border-radius: 100%;
    margin: 1rem auto;
    overflow: hidden;
    img {
      width: 100%;
    }
  }
  &__quote {
    font-style: italic;
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 2;
    overflow: hidden;
  }
}
.carousel__indicator {
  display: inline-block;
  height: 0.8rem;
  width: 0.8rem;
  margin: 0 0.3rem;
  border-radius: 100%;
  border: 1px solid $text-dark;
  &.active {
    background-color: $text-dark;
  }
}
</style>
