<template>
  <main>
    <!-- JUMBOTRON -->
    <section class="jumbo text-white d-flex align-items-center">
      <div class="container">
        <div class="row row-cols-2">
          <div class="col">
            <h2>SEM Campaigns made simple with Avada</h2>
            <p class="my-4">
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Amet
              expedita autem hic quibusdam quia molestiae.
            </p>
            <a href="#" class="btn btn-primary link-light">Buy Avada Now</a>
            <a href="#" class="btn btn-secondary ms-2">Contact us</a>
          </div>
        </div>
      </div>
    </section>
    <section class="template-promo"></section>
    <section class="services"></section>
    <section class="our-work"></section>
    <section class="pricing"></section>
    <section class="news"></section>
    <section class="testimonials"></section>
    <section class="cta"></section>
  </main>
</template>

<script>
export default {
  name: "AppMain",
};
</script>

<style lang="scss" scoped>
.jumbo {
  background-image: url("../assets/images/1-hero-image.png");
  background-size: cover;
  background-position: center;
  height: 100vh;
}
h2 {
  font-size: 3rem;
  font-weight: 700;
}
</style>
