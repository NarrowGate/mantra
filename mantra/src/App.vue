<template>
  <div id="app">
    <div class="page-loading active">
      <div class="page-loading-inner">
        <div class="page-spinner"></div>
        <span>Loading...</span>
      </div>
    </div>
    <main class="page-wrapper">
      <!-- Sign In Modal-->
      <div class="modal fade" id="modal-signin" tabindex="-1">
        <div class="modal-dialog modal-dialog-centered" role="document">
          <div class="modal-content border-0">
            <div class="view show" id="modal-signin-view">
              <div class="modal-header border-0 bg-dark px-4">
                <h4 class="modal-title text-light">Sign in</h4>
                <button
                  class="btn-close btn-close-white"
                  type="button"
                  data-bs-dismiss="modal"
                  aria-label="btn-close "
                ></button>
              </div>
              <div class="modal-body px-4">
                <p class="fs-ms text-muted">
                  Sign in to your account using email and password provided
                  during registration.
                </p>
                <form class="needs-validation" novalidate>
                  <div class="mb-3">
                    <div class="input-group">
                      <i
                        class="ai-mail position-absolute top-50 start-0 translate-middle-y ms-3"
                      ></i>
                      <input
                        class="form-control rounded"
                        type="email"
                        placeholder="Email"
                        required
                      />
                    </div>
                  </div>
                  <div class="mb-3">
                    <div class="input-group">
                      <i
                        class="ai-lock position-absolute top-50 start-0 translate-middle-y ms-3"
                      ></i>
                      <div class="password-toggle w-100">
                        <input
                          class="form-control"
                          type="password"
                          placeholder="Password"
                          required
                        />
                        <label
                          class="password-toggle-btn"
                          aria-label="Show/hide password"
                        >
                          <input
                            class="password-toggle-check"
                            type="checkbox"
                          /><span class="password-toggle-indicator"></span>
                        </label>
                      </div>
                    </div>
                  </div>
                  <div
                    class="d-flex justify-content-between align-items-center mb-3 mb-3"
                  >
                    <div class="form-check">
                      <input
                        class="form-check-input"
                        type="checkbox"
                        id="keep-signed"
                      />
                      <label class="form-check-label fs-sm" for="keep-signed"
                        >Keep me signed in</label
                      >
                    </div>
                    <a
                      class="nav-link-style fs-ms"
                      href="password-recovery.html"
                      >Forgot password?</a
                    >
                  </div>
                  <button class="btn btn-primary d-block w-100" type="submit">
                    Sign in
                  </button>
                  <p class="fs-sm pt-3 mb-0">
                    Don't have an account?
                    <a href="#" class="fw-medium" data-view="#modal-signup-view"
                      >Sign up</a
                    >
                  </p>
                </form>
              </div>
            </div>
            <div class="view" id="modal-signup-view">
              <div class="modal-header border-0 bg-dark px-4">
                <h4 class="modal-title text-light">Sign up</h4>
                <button
                  class="btn-close btn-close-white"
                  type="button"
                  data-bs-dismiss="modal"
                  aria-label="btn-close"
                ></button>
              </div>
              <div class="modal-body px-4">
                <p class="fs-ms text-muted">
                  Registration takes less than a minute but gives you full
                  control over your orders.
                </p>
                <form class="needs-validation" novalidate>
                  <div class="mb-3">
                    <input
                      class="form-control"
                      type="text"
                      placeholder="Full name"
                      required
                    />
                  </div>
                  <div class="mb-3">
                    <input
                      class="form-control"
                      type="text"
                      placeholder="Email"
                      required
                    />
                  </div>
                  <div class="mb-3 password-toggle">
                    <input
                      class="form-control"
                      type="password"
                      placeholder="Password"
                      required
                    />
                    <label
                      class="password-toggle-btn"
                      aria-label="Show/hide password"
                    >
                      <input
                        class="password-toggle-check"
                        type="checkbox"
                      /><span class="password-toggle-indicator"></span>
                    </label>
                  </div>
                  <div class="mb-3 password-toggle">
                    <input
                      class="form-control"
                      type="password"
                      placeholder="Confirm password"
                      required
                    />
                    <label
                      class="password-toggle-btn"
                      aria-label="Show/hide password"
                    >
                      <input
                        class="password-toggle-check"
                        type="checkbox"
                      /><span class="password-toggle-indicator"></span>
                    </label>
                  </div>
                  <button class="btn btn-primary d-block w-100" type="submit">
                    Sign up
                  </button>
                  <p class="fs-sm pt-3 mb-0">
                    Already have an account?
                    <a href="#" class="fw-medium" data-view="#modal-signin-view"
                      >Sign in</a
                    >
                  </p>
                </form>
              </div>
            </div>
            <div class="modal-body text-center px-4 pt-2 pb-4">
              <hr class="my-0" />
              <p class="fs-sm fw-medium text-heading pt-4">Or sign in with</p>
              <a class="btn-social bs-facebook bs-lg mx-1 mb-2" href="#"
                ><i class="ai-facebook"></i></a
              ><a class="btn-social bs-twitter bs-lg mx-1 mb-2" href="#"
                ><i class="ai-twitter"></i></a
              ><a class="btn-social bs-instagram bs-lg mx-1 mb-2" href="#"
                ><i class="ai-instagram"></i></a
              ><a class="btn-social bs-google bs-lg mx-1 mb-2" href="#"
                ><i class="ai-google"></i
              ></a>
            </div>
          </div>
        </div>
      </div>
      <!-- Navbar Floating light for Index page only-->
      <!-- Remove "navbar-sticky" class to make navigation bar scrollable with the page.-->
      <m-header />

      <!-- Page content-->
      <!-- Intro-->
      <section class="container my-lg-2 pt-5 pb-lg-7">
        <div class="row align-items-center">
          <div class="col-lg-5 py-3 py-lg-0">
            <h1>Our goals. Our mission.</h1>
            <h2 class="h3">How we help other companies to grow.</h2>
            <div class="py-4">
              <p class="callout">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud.</p>
            </div>
              <!-- <a class="btn-video btn-video-primary btn-video-sm me-3" href="https://www.youtube.com/watch?v=hTu0a4o97dU"></a>
              <span class="fs-sm text-muted">Get to know us better</span> -->
          </div>
          <div class="col-xl-6 col-lg-7 offset-xl-1 position-relative">
            <div class="py-5" style="min-height: 543px;">
              <div class="d-none d-lg-block position-absolute bg-no-repeat bg-position-center h-100" style="top: 0; left: -45px; width: 646px; background-image: url(img/pages/about/bg-shape.svg);"></div>
              <div class="row g-0 mx-n2 pt-lg-4">
                <div class="col-sm-4 px-2 mb-3">
                  <a class="card h-100 card-body py-5 justify-content-center border-0 shadow-lg text-center" href="#">
                    <i class="ai-zap text-primary h1 mb-3"></i>
                    <h3 class="h5 mb-0">$199</h3>
                  </a>
                </div>
                <div class="col-sm-8 px-2 mb-3">
                  <a class="card card-body py-5 border-0 shadow-lg text-center mb-3" href="#">
                    <i class="ai-pie-chart text-danger h1 mb-3"></i>
                    <h3 class="h5 mb-0">$61 - Cashback or Refund</h3>
                  </a>
                  <a class="card card-body py-5 border-0 shadow-lg text-center" href="#">
                    <i class="ai-refresh-ccw text-info h1 mb-3"></i>
                    <h3 class="h5 mb-0">Contact number</h3>
                  </a>
                </div>                
                <!-- <div class="col-sm-4 px-2 mb-3">
                  <a class="card card-body py-5 border-0 shadow-lg text-center mb-3" href="#">
                    <i class="ai-pie-chart text-danger h1 mb-3"></i>
                    <h3 class="h5 mb-0">$61</h3>
                  </a>
                  <a class="card card-body py-5 border-0 shadow-lg text-center" href="#">
                    <i class="ai-refresh-ccw text-info h1 mb-3"></i>
                    <h3 class="h5 mb-0">Cashback or</h3>
                  </a>
                </div>
                <div class="col-sm-4 px-2 mb-3">
                  <a class="card card-body py-5 border-0 shadow-lg text-center mb-3" href="#">
                    <i class="ai-folder-plus text-success h1 mb-3"></i>
                    <h3 class="h5 mb-0">Share</h3>
                  </a>
                  <a class="card card-body py-5 border-0 shadow-lg text-center" href="#">
                    <i class="ai-share text-warning h1 mb-3"></i>
                    <h3 class="h5 mb-0">Rebook</h3>
                  </a>
                </div> -->
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- Statistics-->
      <section class="bg-secondary py-5 mt-n4 mb-6 mt-lg-0 mb-lg-7">
        <div class="container py-3">
          <div class="row">
            <div class="col-md-4 col-sm-6 text-center py-4">
              <h3 class="display-4">10+</h3>
              <p class="text-muted mb-0">Years of experience</p>
            </div>
            <div class="col-md-4 col-sm-6 text-center py-4">
              <h3 class="display-4">2500+</h3>
              <p class="text-muted mb-0">Tests</p>
            </div>
            <div class="col-md-4 col-sm-6 text-center py-4">
              <h3 class="display-4">100%</h3>
              <p class="text-muted mb-0">Pass Rate</p>
            </div>
            <!-- <div class="col-md-3 col-sm-6 text-center py-3">
              <h3 class="display-4">100</h3>
              <p class="text-muted mb-0">Successfully completed projects</p>
            </div> -->
          </div>
        </div>
      </section>
      <!-- Regions-->
      <section class="container pb-5 pb-lg-6">
        <h2 class="mb-5 text-center">Regions we cover</h2>
        <div class="row">
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter">
            <!-- <a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              </a> -->
              <div class="mantra-area">
                <h3>
                  Logan
                </h3>
              </div>
              <!-- <div class="card-body px-1 py-0 text-center"></div> -->
            
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter">
              <div class="mantra-area">
                <h3>
                  Greenslopes
                </h3>
              </div>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter">
              <div class="mantra-area">
                <h3>
                  Toowong
                </h3>
              </div>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter">
              <div class="mantra-area">
                <h3>
                  Sherwood
                </h3>
              </div>
          </div>                              
          <!-- <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter"><a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              <div class="card-body px-1 py-0 text-center">
                <div class="swap-image"><img class="swap-to" src="img/shop/brands/02_color.png" alt="Brand logo" width="150"><img class="swap-from" src="img/shop/brands/02_gray.png" alt="Brand logo" width="150"></div>
              </div></a>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter"><a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              <div class="card-body px-1 py-0 text-center">
                <div class="swap-image"><img class="swap-to" src="img/shop/brands/03_color.png" alt="Brand logo" width="150"><img class="swap-from" src="img/shop/brands/03_gray.png" alt="Brand logo" width="150"></div>
              </div></a>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter"><a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              <div class="card-body px-1 py-0 text-center">
                <div class="swap-image"><img class="swap-to" src="img/shop/brands/04_color.png" alt="Brand logo" width="150"><img class="swap-from" src="img/shop/brands/04_gray.png" alt="Brand logo" width="150"></div>
              </div></a>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter"><a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              <div class="card-body px-1 py-0 text-center">
                <div class="swap-image"><img class="swap-to" src="img/shop/brands/05_color.png" alt="Brand logo" width="150"><img class="swap-from" src="img/shop/brands/05_gray.png" alt="Brand logo" width="150"></div>
              </div></a>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter"><a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              <div class="card-body px-1 py-0 text-center">
                <div class="swap-image"><img class="swap-to" src="img/shop/brands/06_color.png" alt="Brand logo" width="150"><img class="swap-from" src="img/shop/brands/06_gray.png" alt="Brand logo" width="150"></div>
              </div></a>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter"><a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              <div class="card-body px-1 py-0 text-center">
                <div class="swap-image"><img class="swap-to" src="img/shop/brands/07_color.png" alt="Brand logo" width="150"><img class="swap-from" src="img/shop/brands/07_gray.png" alt="Brand logo" width="150"></div>
              </div></a>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter"><a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              <div class="card-body px-1 py-0 text-center">
                <div class="swap-image"><img class="swap-to" src="img/shop/brands/08_color.png" alt="Brand logo" width="150"><img class="swap-from" src="img/shop/brands/08_gray.png" alt="Brand logo" width="150"></div>
              </div></a>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter"><a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              <div class="card-body px-1 py-0 text-center">
                <div class="swap-image"><img class="swap-to" src="img/shop/brands/09_color.png" alt="Brand logo" width="150"><img class="swap-from" src="img/shop/brands/09_gray.png" alt="Brand logo" width="150"></div>
              </div></a>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter"><a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              <div class="card-body px-1 py-0 text-center">
                <div class="swap-image"><img class="swap-to" src="img/shop/brands/10_color.png" alt="Brand logo" width="150"><img class="swap-from" src="img/shop/brands/10_gray.png" alt="Brand logo" width="150"></div>
              </div></a>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter"><a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              <div class="card-body px-1 py-0 text-center">
                <div class="swap-image"><img class="swap-to" src="img/shop/brands/11_color.png" alt="Brand logo" width="150"><img class="swap-from" src="img/shop/brands/11_gray.png" alt="Brand logo" width="150"></div>
              </div></a>
          </div>
          <div class="col-md-3 col-sm-4 col-6 mb-grid-gutter"><a class="card border-0 shadow card-hover py-3 py-sm-4" href="#">
              <div class="card-body px-1 py-0 text-center">
                <div class="swap-image"><img class="swap-to" src="img/shop/brands/12_color.png" alt="Brand logo" width="150"><img class="swap-from" src="img/shop/brands/12_gray.png" alt="Brand logo" width="150"></div>
              </div></a>
          </div> -->
        </div>
      </section>      
      <!-- Team-->
      <section class="container mb-5 pb-3 pb-lg-0 mb-lg-7">
        <h2 class="pb-4 mb-4 text-center">People behind our success</h2>
        <div class="row mb-3">
          <div class="col-lg-3 col-md-4 col-sm-6 mb-grid-gutter">
            <div class="card card-curved-body card-hover border-0 shadow mx-auto" style="max-width: 21rem;"><a class="card-floating-icon" href="mailto:sarah.cole@example.com"><i class="ai-mail"></i></a>
              <br>
              <div class="card-body text-center">
                <h3 class="h6 card-title mb-2">Aby Cherian</h3>
                <p class="fs-xs text-body mb-0">CEO, Co-Founder</p>
              </div>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 col-sm-6 mb-grid-gutter">
            <div class="card card-curved-body card-hover border-0 shadow mx-auto" style="max-width: 21rem;"><a class="card-floating-icon" href="mailto:charlie.welch@example.com"><i class="ai-mail"></i></a>
              <br>
              <div class="card-body text-center">
                <h3 class="h6 card-title mb-2">Milan</h3>
                <p class="fs-xs text-body mb-0">CTO, Co-Founder</p>
              </div>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 col-sm-6 mb-grid-gutter">
            <div class="card card-curved-body card-hover border-0 shadow mx-auto" style="max-width: 21rem;"><a class="card-floating-icon" href="mailto:emma.brown@example.com"><i class="ai-mail"></i></a>
              <br>
              <div class="card-body text-center">
                <h3 class="h6 card-title mb-2">Manasa</h3>
                <p class="fs-xs text-body mb-0">Director of Marketing</p>
              </div>
            </div>
          </div>
          <div class="col-lg-3 col-md-4 col-sm-6 mb-grid-gutter">
            <div class="card card-curved-body card-hover border-0 shadow mx-auto" style="max-width: 21rem;"><a class="card-floating-icon" href="mailto:rosalie.lyons@example.com"><i class="ai-mail"></i></a>
              <br>
              <div class="card-body text-center">
                <h3 class="h6 card-title mb-2">Susan</h3>
                <p class="fs-xs text-body mb-0">Financial Director</p>
              </div>
            </div>
          </div>
        </div>
        <!-- <div class="card card-body py-5 text-center text-md-end">
          <div class="d-md-flex justify-content-center align-items-center">
            <div class="mb-4 mb-md-0 me-md-5 me-lg-6 me-xl-7">
              <h3>Want to be part of our team? We are hiring</h3>
              <p class="text-muted mb-0">Check our current opennings and submit your application</p>
            </div><a class="btn btn-gradient" href="#">Submit your application</a>
          </div>
        </div> -->
      </section>
    </main>
    <m-footer/>
    <!-- Back to top button--><a
      class="btn-scroll-top"
      href="#top"
      data-scroll
      data-fixed-element
      ><span class="btn-scroll-top-tooltip text-muted fs-sm me-2">Top</span
      ><i class="btn-scroll-top-icon ai-arrow-up"> </i
    ></a>
  </div>
</template>
<script>
import MHeader from '@/components/MHeader.vue';
import MFooter from '@/components/MFooter.vue';
// import Intro from '@/components/Intro.vue';
// import Demos from '@/components/Demos.vue';
// import Komponents from '@/components/Komponents.vue';
// import InnerPages from '@/components/InnerPages.vue';
// import MobileInterface from '@/components/MobileInterface.vue';
// import Features from '@/components/Features.vue';


export default {
  components: {
    MHeader,
    MFooter,
    // Demos,
    // Intro,
    // Komponents,
    // InnerPages,
    // MobileInterface,
    // Features
  },
  created() {
    (function () {
      window.onload = function () {
        var preloader = document.querySelector('.page-loading');
        preloader.classList.remove('active');
        setTimeout(function () {
          preloader.remove();
        }, 2000);
      };
    })();
  },
};
</script>
<style lang="scss">
$mantraYellow: #FFCC00;
$mantraBlack: #000000;
$mantraPurple: #756df4;
$mantraLightPurple: #c5c2fb;

body {
  background-color: $mantraBlack;
  h1 {
    color: $mantraYellow;
  }
  h2 {
    color: $mantraPurple !important;
  }  
  .mantra-area {
    background: url("./assets/images/map.jpg") no-repeat;
    border-radius: 10px;
    height: 150px;
    display: flex;
    justify-content: center;
    align-items: center;
    h3 {
      font-size: 33px;
    }
  }
  .callout {
    border-color: $mantraYellow;
  }
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $mantraLightPurple;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
// $primaryColor: #e75500;
// $primaryColorHvr: #e85400;

// $primaryTypeColor: #d2c6b4;

// $secondaryColor: #4b4a48;
// $secondaryTypeColor: white;
// $formErrorRed: #e49191;

// $tertiaryColor: #d3c6b5;
// $tertiaryTypeColor: #5d2814;
