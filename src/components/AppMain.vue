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
    <!-- TEMPLATE PROMO -->
    <section class="template-promo">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-6 text-center">
            <h3>Meet the new agency SEO Template From the Avada Team</h3>
            <p class="text-muted pb-5">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Voluptatem atque aliquam est eos expedita beatae.
            </p>
          </div>
        </div>
        <div class="row gx-3 text-center">
          <div class="col-4">
            <div class="bg-white p-5">
              <i class="fas fa-road"></i>
              <h4>Establish Goals</h4>
              <p class="text-muted">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi
                eius, dicta voluptatum dolore sed pariatur! Expedita facilis
                assumenda natus fugit!
              </p>
            </div>
          </div>
          <div class="col-4">
            <div class="bg-white p-5">
              <i class="fas fa-video"></i>
              <h4>Work with a Team</h4>
              <p class="text-muted">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi
                eius, dicta voluptatum dolore sed pariatur! Expedita facilis
                assumenda natus fugit!
              </p>
            </div>
          </div>
          <div class="col-4">
            <div class="bg-white p-5">
              <i class="fas fa-tint"></i>
              <h4>Get Results</h4>
              <p class="text-muted">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi
                eius, dicta voluptatum dolore sed pariatur! Expedita facilis
                assumenda natus fugit!
              </p>
            </div>
          </div>
        </div>
        <img
          src="../assets/images/agency-seo-desk-front.jpg"
          alt="A nice desk"
        />
      </div>
    </section>
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
@import "../style/variables.scss";
@import "../style/common.scss";
img {
  max-width: 100%;
}
h2 {
  font-size: 3rem;
  font-weight: 700;
}
h3 {
  font-size: 2rem;
  font-weight: 700;
}
h4 {
  font-size: 1.5rem;
  font-weight: 700;
  margin: 1rem 0;
}
.jumbo {
  background-image: url("../assets/images/1-hero-image.png");
  background-size: cover;
  background-position: center;
  height: 100vh;
}
.template-promo {
  background-color: $background-light;
  padding-top: 4rem;
  i {
    font-size: 3rem;
    color: $primary;
  }
}
</style>
