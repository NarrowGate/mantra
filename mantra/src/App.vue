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
      <intro />
      <!-- Demos-->
      <demos />
      <!-- Components-->
      <komponents />
      <!-- Inner Pages-->
      <inner-pages />
      <!-- Mobile Interface-->
      <mobile-interface />
      <!-- Features-->
      <features />
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
import Intro from '@/components/Intro.vue';
import Komponents from '@/components/Komponents.vue';
import InnerPages from '@/components/InnerPages.vue';
import MobileInterface from '@/components/MobileInterface.vue';
import Features from '@/components/Features.vue';


export default {
  components: {
    MHeader,
    MFooter,
    Intro,
    Komponents,
    InnerPages,
    MobileInterface,
    Features
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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
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
