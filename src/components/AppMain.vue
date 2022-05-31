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
    <!-- SERVICES -->
    <section class="services text-white">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-6 text-center">
            <h3>See Our Top Notch Services</h3>
            <p class="pb-5">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Voluptatem atque aliquam est eos expedita beatae.
            </p>
          </div>
        </div>
        <div class="row gx-3 text-center">
          <div class="col-3">
            <div class="services__card bg-blue p-5">
              <i class="fab fa-google"></i>
              <h4>Google SEO</h4>
              <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi
                eius, dicta voluptatum dolore sed pariatur! Expedita facilis
                assumenda natus fugit!
              </p>
              <a href="#">Read more ></a>
            </div>
          </div>
          <div class="col-3">
            <div class="services__card bg-blue p-5">
              <i class="fas fa-cog"></i>
              <h4>Brand Strategy</h4>
              <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi
                eius, dicta voluptatum dolore sed pariatur! Expedita facilis
                assumenda natus fugit!
              </p>
              <a href="#">Read more ></a>
            </div>
          </div>
          <div class="col-3">
            <div class="services__card bg-blue p-5">
              <i class="fas fa-building"></i>
              <h4>Local SEO</h4>
              <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi
                eius, dicta voluptatum dolore sed pariatur! Expedita facilis
                assumenda natus fugit!
              </p>
              <a href="#">Read more ></a>
            </div>
          </div>
          <div class="col-3">
            <div class="services__card bg-blue p-5">
              <i class="fas fa-chart-bar"></i>
              <h4>SEO Analysis</h4>
              <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi
                eius, dicta voluptatum dolore sed pariatur! Expedita facilis
                assumenda natus fugit!
              </p>
              <a href="#">Read more ></a>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- OUR WORK -->
    <section class="our-work">
      <div class="container text-center">
        <div class="row justify-content-center">
          <div class="col-6">
            <h3>Our Work</h3>
            <p class="text-muted pb-5">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Voluptatem atque aliquam est eos expedita beatae.
            </p>
          </div>
        </div>
        <div class="row g-3">
          <div
            v-for="(item, index) in caseStudyImgURLs"
            :key="index"
            class="col-4"
          >
            <img :src="require(`../assets/images/${item}`)" alt="" />
          </div>
        </div>
        <a href="#" class="btn btn-primary link-light my-4">View Our Work</a>
      </div>
    </section>
    <!-- PRICING -->
    <section class="pricing">
      <div class="container">
        <div class="row justify-content-center text-white">
          <div class="col-6 text-center">
            <h3>Our Plans</h3>
            <p class="pb-5">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Voluptatem atque aliquam est eos expedita beatae.
            </p>
          </div>
        </div>
        <div class="row gx-3 text-center">
          <div class="col-3">
            <div class="pricing__card bg-white p-5">
              <h4>Standard</h4>
              <div class="price">
                <span class="currency">$</span
                ><span class="integer-part">19</span
                ><sup class="decimal-part">99</sup
                ><span class="period text-muted">monthly</span>
              </div>
              <p>5 Projects</p>
              <p>5 GB Storage</p>
              <p>Unlimited Users</p>
              <a class="btn btn-outline-dark" href="#">START TODAY</a>
            </div>
          </div>
          <div class="col-3">
            <div class="pricing__card bg-white p-5">
              <h4>Premium</h4>
              <div class="price">
                <span class="currency">$</span
                ><span class="integer-part">29</span
                ><sup class="decimal-part">99</sup
                ><span class="period text-muted">monthly</span>
              </div>
              <p>10 Projects</p>
              <p>15 GB Storage</p>
              <p>Unlimited Users</p>
              <a class="btn btn-outline-dark" href="#">START TODAY</a>
            </div>
          </div>
          <div class="col-3">
            <div class="pricing__card bg-white p-5">
              <h4>Professional</h4>
              <div class="price">
                <span class="currency">$</span
                ><span class="integer-part">39</span
                ><sup class="decimal-part">99</sup
                ><span class="period text-muted">monthly</span>
              </div>
              <p>15 Projects</p>
              <p>30 GB Storage</p>
              <p>Unlimited Users</p>
              <a class="btn btn-primary text-light" href="#">START TODAY</a>
            </div>
          </div>
          <div class="col-3">
            <div class="pricing__card bg-white p-5">
              <h4>Extreme</h4>
              <div class="price">
                <span class="currency">$</span
                ><span class="integer-part">59</span
                ><sup class="decimal-part">99</sup
                ><span class="period text-muted">monthly</span>
              </div>
              <p>Unlimited Projects</p>
              <p>Unlimited Storage</p>
              <p>Unlimited Users</p>
              <a class="btn btn-outline-dark" href="#">START TODAY</a>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- NEWS -->
    <section class="news">
      <div class="container text-center">
        <div class="row justify-content-center">
          <div class="col-6">
            <h3>Our News</h3>
            <p class="text-muted pb-5">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Voluptatem atque aliquam est eos expedita beatae.
            </p>
          </div>
        </div>
        <div class="row g-3">
          <div class="col-4">
            <div class="news__card">
              <img
                src="../assets/images/related-service-2-700x441.jpg"
                alt=""
              />
              <h4 class="text-primary">Why You Need a SEO Agency Now</h4>
              <p class="news__date text-muted">November 1st, 2017</p>
              <p class="text-muted">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Qui
                soluta vero id totam maiores repellendus animi porro in iusto
                nemo?
              </p>
            </div>
          </div>
          <div class="col-4">
            <div class="news__card">
              <img
                src="../assets/images/related-service-4-700x441.jpg"
                alt=""
              />
              <h4 class="text-primary">SEO Tips for your Startup</h4>
              <p class="news__date text-muted">November 1st, 2017</p>
              <p class="text-muted">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Qui
                soluta vero id totam maiores repellendus animi porro in iusto
                nemo?
              </p>
            </div>
          </div>
          <div class="col-4">
            <div class="news__card">
              <img src="../assets/images/blog-post-6-700x441.jpg" alt="" />
              <h4 class="text-primary">Image Optimization for Your Site</h4>
              <p class="news__date text-muted">November 1st, 2017</p>
              <p class="text-muted">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Qui
                soluta vero id totam maiores repellendus animi porro in iusto
                nemo?
              </p>
            </div>
          </div>
        </div>
        <a href="#" class="btn btn-primary link-light my-4">Go to News</a>
      </div>
    </section>
    <section class="testimonials">
      <div class="container text-center">
        <div class="row justify-content-center">
          <div class="col-6">
            <h3 class="mb-3">What Our Clients Say</h3>
          </div>
        </div>
        <div class="row justify-content-center">
          <div class="col-6">
            <AppCarousel :slides="testimonialsCarousel" />
          </div>
        </div>
        <hr class="my-5" />
        <div class="row justify-content-around">
          <div class="col-3">
            <img
              class="partner-img"
              src="../assets/images/clients_partner_5-200x202.png"
              alt=""
            />
          </div>
          <div class="col-3">
            <img
              class="partner-img"
              src="../assets/images/clients_partner_6-200x202.png"
              alt=""
            />
          </div>
          <div class="col-3">
            <img
              class="partner-img"
              src="../assets/images/clients_partner_1-200x202.png"
              alt=""
            />
          </div>
          <div class="col-3">
            <img
              class="partner-img"
              src="../assets/images/clients_partner_2-200x202.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </section>
    <section class="cta"></section>
  </main>
</template>

<script>
import AppCarousel from "./AppCarousel.vue";
export default {
  name: "AppMain",
  components: { AppCarousel },
  data() {
    return {
      caseStudyImgURLs: [
        "case-study-gallery-3-1.jpg",
        "case-study-gallery-2.jpg",
        "case-study-gallery-1-1.jpg",
        "case-study-gallery-4-1.jpg",
        "case-study-gallery-5-1.jpg",
        "case-study-gallery-6-1.jpg",
      ],
      testimonialsCarousel: [
        {
          img: "testimonials-2.jpg",
          quote:
            " Ability proceeds from a fusion of skills, knowledge, understanding and imagination, consolidated by experience.",
          name: "Luis Desalvo",
          org: "CREO TECH",
        },
        {
          img: "testimonials-1.jpg",
          quote:
            " Beauty is when you can appreciate yourself. When you love yourself, that’s when you’re most beautiful. Beauty is when you can appreciate yourself. When you love yourself, that’s when you’re most beautiful. Beauty is when you can appreciate yourself. When you love yourself, that’s when you’re most beautiful.",
          name: "Shelia McCourtney",
          org: "ARCHITECT",
        },
      ],
    };
  },
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
  font-size: 1.2rem;
  font-weight: 700;
  margin: 1rem 0;
}

a {
  text-decoration: none;
}

.bg-blue {
  background-color: $blue;
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
.services {
  background-color: $background-darkblue;
  background-image: url("../assets/images/pattern_background.png");
  background-size: contain;
  padding: 4rem 0 6rem;
  &__card {
    height: 100%;
  }
  i {
    font-size: 3rem;
    color: $primary;
  }
}
.our-work {
  background-color: $background-light;
  padding-top: 4rem;
}
.pricing {
  background-image: url("../assets/images/background1.jpg");
  background-size: cover;
  padding: 4rem 0 6rem;
  &__card {
    height: 100%;
  }
  p {
    font-size: 0.9rem;
  }
  .price {
    position: relative;
    .currency {
      font-size: 1.5rem;
      position: relative;
      top: -1rem;
      left: 0;
    }
    .integer-part {
      color: $text-pricing-blue;
      font-size: 3rem;
      font-weight: bold;
    }
    .decimal-part {
      color: $text-pricing-blue;
      font-size: 1rem;
      font-weight: bold;
      position: relative;
      top: -1.2rem;
      left: 0;
    }
    .period {
      font-style: italic;
      font-size: 0.8rem;
      margin-left: -1rem;
    }
  }
}
.news {
  padding: 4rem 0 6rem;
  background-color: $background-light;
  &__date {
    font-size: 0.8rem;
  }
}
.testimonials {
  background-color: white;
  padding: 4rem 0;
  .partner-img {
    max-width: 100px;
  }
}
</style>
