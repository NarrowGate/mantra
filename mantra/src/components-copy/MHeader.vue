<template>
  <header
    class="header navbar navbar-expand-lg navbar-dark navbar-floating navbar-sticky"
    data-fixed-element
  >
    <div class="container px-0 px-xl-3">
      <button
        class="navbar-toggler ms-n2 me-2"
        type="button"
        data-bs-toggle="offcanvas"
        data-bs-target="#primaryMenu"
      >
        <span class="navbar-toggler-icon"></span></button
      ><a
        class="navbar-brand flex-shrink-0 order-lg-1 mx-auto ms-lg-0 pe-lg-2 me-lg-4"
        href="index.html"
        ><img
          class="navbar-floating-logo d-none d-lg-block"
          src="img/logo/logo-light.png"
          alt="Around"
          width="153" /><img
          class="navbar-stuck-logo"
          src="img/logo/logo-dark.png"
          alt="Around"
          width="153" /><img
          class="d-lg-none"
          src="img/logo/logo-icon.png"
          alt="Around"
          width="58"
      /></a>
      <div class="d-flex align-items-center order-lg-3 ms-lg-auto">
        <a
          class="btn btn-primary"
          href="https://themes.getbootstrap.com/product/around-multipurpose-template-ui-kit/"
          target="_blank"
          rel="noopener"
          ><i class="ai-shopping-cart fs-lg me-2"></i>Buy
          <span class="d-none d-lg-inline">Template</span></a
        >
      </div>
      <div class="offcanvas offcanvas-collapse order-lg-2" id="primaryMenu">
        <div class="offcanvas-cap navbar-shadow">
          <h5 class="mt-1 mb-0">Menu</h5>
          <button
            class="btn-close lead"
            type="button"
            data-bs-dismiss="offcanvas"
            aria-label="Close"
          ></button>
        </div>
        <div class="offcanvas-body">
          <!-- Menu-->
          <ul class="navbar-nav">
            <li class="nav-item dropdown dropdown-mega">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                data-bs-toggle="dropdown"
                >Demos</a
              >
              <div class="dropdown-menu">
                <a
                  class="dropdown-column dropdown-column-img bg-secondary"
                  href="index.html"
                  style="background-image: url(img/demo/menu-banner.jpg)"
                ></a>
                <div class="dropdown-column">
                  <a class="dropdown-item" href="index.html"
                    >Web Template Presentation</a
                  ><a
                    class="dropdown-item"
                    href="demo-business-consulting.html"
                    >Business Consulting</a
                  ><a class="dropdown-item" href="demo-shop-homepage.html"
                    >Shop Homepage</a
                  ><a
                    class="dropdown-item"
                    href="demo-booking-directory.html"
                    >Booking / Directory</a
                  ><a class="dropdown-item" href="demo-creative-agency.html"
                    >Creative Agency</a
                  ><a class="dropdown-item" href="demo-web-studio.html"
                    >Web Studio</a
                  ><a
                    class="dropdown-item"
                    href="demo-product-software.html"
                    >Product Landing - Software</a
                  >
                </div>
                <div class="dropdown-column">
                  <a class="dropdown-item" href="demo-product-gadget.html"
                    >Product Landing - Gadget</a
                  ><a class="dropdown-item" href="demo-mobile-app.html"
                    >Mobile App Showcase</a
                  ><a class="dropdown-item" href="demo-coworking-space.html"
                    >Coworking Space</a
                  ><a class="dropdown-item" href="demo-event-landing.html"
                    >Event Landing</a
                  ><a class="dropdown-item" href="demo-marketing-seo.html"
                    >Digital Marketing &amp; SEO</a
                  ><a class="dropdown-item" href="demo-food-blog.html"
                    >Food Blog</a
                  ><a
                    class="dropdown-item"
                    href="demo-personal-portfolio.html"
                    >Personal Portfolio</a
                  >
                </div>
              </div>
            </li>
            <li class="nav-item dropdown dropdown-mega">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                data-bs-toggle="dropdown"
                >Templates</a
              >
              <div class="dropdown-menu">
                <div class="dropdown-column mb-2 mb-lg-0">
                  <h5 class="dropdown-header">Blog</h5>
                  <a class="dropdown-item" href="blog-grid-rs.html"
                    >Grid Right Sidebar</a
                  ><a class="dropdown-item" href="blog-grid-ls.html"
                    >Grid Left Sidebar</a
                  ><a class="dropdown-item" href="blog-grid-ns.html"
                    >Grid No Sidebar</a
                  ><a class="dropdown-item" href="blog-list-rs.html"
                    >List Right Sidebar</a
                  ><a class="dropdown-item" href="blog-list-ls.html"
                    >List Left Sidebar</a
                  ><a class="dropdown-item" href="blog-list-ns.html"
                    >List No Sidebar</a
                  ><a class="dropdown-item" href="blog-single-rs.html"
                    >Single Post Right Sidebar</a
                  ><a class="dropdown-item" href="blog-single-ls.html"
                    >Single Post Left Sidebar</a
                  ><a class="dropdown-item" href="blog-single-ns.html"
                    >Single Post No Sidebar</a
                  >
                </div>
                <div class="dropdown-column mb-2 mb-lg-0">
                  <h5 class="dropdown-header">Portfolio</h5>
                  <a class="dropdown-item" href="portfolio-style-1.html"
                    >Grid Style 1</a
                  ><a class="dropdown-item" href="portfolio-style-2.html"
                    >Grid Style 2</a
                  ><a class="dropdown-item" href="portfolio-style-3.html"
                    >Grid Style 3</a
                  ><a
                    class="dropdown-item"
                    href="portfolio-single-side-gallery-grid.html"
                    >Project Side Gallery (Grid)</a
                  ><a
                    class="dropdown-item"
                    href="portfolio-single-side-gallery-list.html"
                    >Project Side Gallery (List)</a
                  ><a
                    class="dropdown-item"
                    href="portfolio-single-carousel.html"
                    >Project Carousel</a
                  ><a
                    class="dropdown-item"
                    href="portfolio-single-wide-gallery.html"
                    >Project Wide Gallery</a
                  >
                </div>
                <div class="dropdown-column mb-2 mb-lg-0">
                  <h5 class="dropdown-header">Shop</h5>
                  <a class="dropdown-item" href="shop-ls.html"
                    >Grid Left Sidebar</a
                  ><a class="dropdown-item" href="shop-rs.html"
                    >Grid Right Sidebar</a
                  ><a class="dropdown-item" href="shop-ns.html"
                    >Grid No Sidebar</a
                  ><a class="dropdown-item" href="shop-single.html"
                    >Single Product</a
                  ><a class="dropdown-item" href="checkout.html"
                    >Cart &amp; Checkout</a
                  ><a class="dropdown-item" href="order-tracking.html"
                    >Order Tracking</a
                  >
                </div>
              </div>
            </li>
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                data-bs-toggle="dropdown"
                >Account</a
              >
              <ul class="dropdown-menu">
                <li class="dropdown">
                  <a
                    class="dropdown-item dropdown-toggle"
                    href="#"
                    data-bs-toggle="dropdown"
                    >Dashboard</a
                  >
                  <ul class="dropdown-menu">
                    <li>
                      <a class="dropdown-item" href="dashboard-orders.html"
                        >Orders</a
                      >
                    </li>
                    <li>
                      <a class="dropdown-item" href="dashboard-sales.html"
                        >Sales</a
                      >
                    </li>
                    <li>
                      <a
                        class="dropdown-item"
                        href="dashboard-messages.html"
                        >Messages</a
                      >
                    </li>
                    <li>
                      <a
                        class="dropdown-item"
                        href="dashboard-followers.html"
                        >Followers</a
                      >
                    </li>
                    <li>
                      <a class="dropdown-item" href="dashboard-reviews.html"
                        >Reviews</a
                      >
                    </li>
                    <li>
                      <a
                        class="dropdown-item"
                        href="dashboard-favorites.html"
                        >Favorites</a
                      >
                    </li>
                  </ul>
                </li>
                <li class="dropdown">
                  <a
                    class="dropdown-item dropdown-toggle"
                    href="#"
                    data-bs-toggle="dropdown"
                    >Account Settings</a
                  >
                  <ul class="dropdown-menu">
                    <li>
                      <a class="dropdown-item" href="account-profile.html"
                        >Profile Info</a
                      >
                    </li>
                    <li>
                      <a class="dropdown-item" href="account-payment.html"
                        >Payment Methods</a
                      >
                    </li>
                    <li>
                      <a
                        class="dropdown-item"
                        href="account-notifications.html"
                        >Notifications</a
                      >
                    </li>
                  </ul>
                </li>
                <li>
                  <a class="dropdown-item" href="signin-illustration.html"
                    >Sign In - Illustration</a
                  >
                </li>
                <li>
                  <a class="dropdown-item" href="signin-image.html"
                    >Sign In - Image</a
                  >
                </li>
                <li>
                  <a class="dropdown-item" href="signin-signup.html"
                    >Sign In - Sign Up</a
                  >
                </li>
                <li>
                  <a class="dropdown-item" href="password-recovery.html"
                    >Password Recovery</a
                  >
                </li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                data-bs-toggle="dropdown"
                >Pages</a
              >
              <ul class="dropdown-menu">
                <li>
                  <a class="dropdown-item" href="about.html">About</a>
                </li>
                <li class="dropdown">
                  <a
                    class="dropdown-item dropdown-toggle"
                    href="#"
                    data-bs-toggle="dropdown"
                    >Contacts</a
                  >
                  <ul class="dropdown-menu">
                    <li>
                      <a class="dropdown-item" href="contacts-v1.html"
                        >Contacts v.1</a
                      >
                    </li>
                    <li>
                      <a class="dropdown-item" href="contacts-v2.html"
                        >Contacts v.2</a
                      >
                    </li>
                    <li>
                      <a class="dropdown-item" href="contacts-v3.html"
                        >Contacts v.3</a
                      >
                    </li>
                  </ul>
                </li>
                <li class="dropdown">
                  <a
                    class="dropdown-item dropdown-toggle"
                    href="#"
                    data-bs-toggle="dropdown"
                    >Help Center</a
                  >
                  <ul class="dropdown-menu">
                    <li>
                      <a class="dropdown-item" href="help-topics.html"
                        >Help Topics</a
                      >
                    </li>
                    <li>
                      <a class="dropdown-item" href="help-single-topic.html"
                        >Single Topic</a
                      >
                    </li>
                    <li>
                      <a
                        class="dropdown-item"
                        href="help-submit-request.html"
                        >Submit a Request</a
                      >
                    </li>
                  </ul>
                </li>
                <li class="dropdown">
                  <a
                    class="dropdown-item dropdown-toggle"
                    href="#"
                    data-bs-toggle="dropdown"
                    >404 Not Found</a
                  >
                  <ul class="dropdown-menu">
                    <li>
                      <a class="dropdown-item" href="404-simple.html"
                        >Simple Text</a
                      >
                    </li>
                    <li>
                      <a class="dropdown-item" href="404-illustration.html"
                        >Illustration</a
                      >
                    </li>
                  </ul>
                </li>
                <li class="dropdown">
                  <a
                    class="dropdown-item dropdown-toggle"
                    href="#"
                    data-bs-toggle="dropdown"
                    >Coming Soon</a
                  >
                  <ul class="dropdown-menu">
                    <li>
                      <a class="dropdown-item" href="coming-soon-image.html"
                        >Image</a
                      >
                    </li>
                    <li>
                      <a
                        class="dropdown-item"
                        href="coming-soon-illustration.html"
                        >Illustration</a
                      >
                    </li>
                  </ul>
                </li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                data-bs-toggle="dropdown"
                >Docs / UI Kit</a
              >
              <ul class="dropdown-menu">
                <li>
                  <a class="dropdown-item" href="docs/dev-setup.html">
                    <div class="d-flex align-items-center">
                      <div class="fs-xl text-muted">
                        <i class="ai-file-text"></i>
                      </div>
                      <div class="ps-3">
                        <span class="d-block text-heading"
                          >Documentation</span
                        ><small class="d-block text-muted"
                          >Kick-start customization</small
                        >
                      </div>
                    </div></a
                  >
                </li>
                <li class="dropdown-divider"></li>
                <li>
                  <a
                    class="dropdown-item"
                    href="components/typography.html"
                  >
                    <div class="d-flex align-items-center">
                      <div class="fs-xl text-muted">
                        <i class="ai-layers"></i>
                      </div>
                      <div class="ps-3">
                        <span class="d-block text-heading"
                          >UI Kit<span class="badge bg-danger ms-2"
                            >50+</span
                          ></span
                        ><small class="d-block text-muted"
                          >Flexible components</small
                        >
                      </div>
                    </div></a
                  >
                </li>
                <li class="dropdown-divider"></li>
                <li>
                  <a class="dropdown-item" href="docs/changelog.html">
                    <div class="d-flex align-items-center">
                      <div class="fs-xl text-muted">
                        <i class="ai-edit"></i>
                      </div>
                      <div class="ps-3">
                        <span class="d-block text-heading"
                          >Changelog<span class="badge bg-success ms-2"
                            >v2.0.0</span
                          ></span
                        ><small class="d-block text-muted"
                          >Regular updates</small
                        >
                      </div>
                    </div></a
                  >
                </li>
                <li class="dropdown-divider"></li>
                <li>
                  <a
                    class="dropdown-item"
                    href="mailto:support@createx.studio"
                  >
                    <div class="d-flex align-items-center">
                      <div class="fs-xl text-muted">
                        <i class="ai-life-buoy"></i>
                      </div>
                      <div class="ps-3">
                        <span class="d-block text-heading">Support</span
                        ><small class="d-block text-muted"
                          >support@createx.studio</small
                        >
                      </div>
                    </div></a
                  >
                </li>
              </ul>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {

}
</script>

<style>

</style>