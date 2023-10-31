<template>
  <div>
    <div class="footer container-md p-0">
      <!-- Footer -->
      <footer class="text-white" style="background-color: #000000">
        <!-- Grid container -->
        <div class="container p-4">
          <!-- Section: Form -->
          <section class="col font-quicksand">
            <form action="">
              <!--Grid row-->
              <div class="row d-flex py-3 justify-content-lg-center">
                <!--Grid column-->
                <div class="col-auto">
                  <p class="pt-2">
                    <strong>Sign up for our newsletter</strong>
                  </p>
                </div>
                <!--Grid column-->

                <!--Grid column-->
                <div class="col-md-5 col-12 font-quicksand">
                  <!-- Email input -->
                  <div class="form-outline form-white mb-3">
                    <input id="form5Example2" type="email" class="form-control" />
                    <label class="form-label" for="form5Example2">Email address</label>
                  </div>
                </div>
                <!--Grid column-->

                <!--Grid column-->
                <div class="col-auto font-quicksand">
                  <!-- Submit button -->
                  <button type="submit" class="btn btn-outline-light mb-4">Subscribe</button>
                </div>
                <!--Grid column-->
              </div>
              <!--Grid row-->
            </form>
          </section>
          <!-- Section: Form -->

          <!-- Section: Text -->
          <section class="my-2 link-section font-quicksand">
            <p class="link-section-caption text-center">we offer best software solution service world-wide.</p>
          </section>
          <!-- Section: Text -->

          <!-- Section: Links -->
          <div class="container">
            <!--Grid row-->
            <div class="row">
              <!--Grid column-->
              <div class="col-md-3 mb-4 mb-md-0 font-quicksand">
                <h5 class="text-capitalize">Contact Us</h5>

                <ul class="list-unstyled mb-0">
                  <li>
                    <a href="mail:Softwareservices@aol.com" target="_blank" class="text-white">Softwareservices@aol.com</a>
                  </li>
                  <li>
                    <a href="tel:+1(812)214-5262" target="_blank" class="text-white">Customer Support : +1(812)214-5262</a>
                  </li>
                </ul>
              </div>
              <!--Grid column-->

              <!--Grid column-->
              <div class="col-lg-3 col-md-6 mb-4 mb-md-0 font-quicksand">
                <h5 class="text-capitalize">Sponsors</h5>

                <ul class="list-unstyled mb-0">
                  <li>
                    <a href="https://coinmarketcap.com/" target="_blank" class="text-white">CoinMarketCap</a>
                  </li>
                  <li>
                    <a href="https://www.wsj.com/" target="_blank" class="text-white">WallStreet Investors</a>
                  </li>
                </ul>
              </div>
              <!--Grid column-->

              <!--Grid column-->
              <div class="col-lg-3 col-md-6 mb-4 mb-md-0 font-quicksand">
                <h5 class="text-capitalize">Affiliates</h5>

                <ul class="list-unstyled mb-0">
                  <li>
                    <a href="https://githubcom/" target="_blank" class="text-white">Github</a>
                  </li>
                  <li>
                    <a href="https://netlify.com/" target="_blank" class="text-white">netlify.com</a>
                  </li>
                </ul>
              </div>
              <!--Grid column-->

              <!--Grid column-->
              <div class="col-lg-3 col-md-6 mb-4 mb-md-0 font-quicksand">
                <h5 class="text-capitalize">Blog</h5>

                <ul class="list-unstyled mb-0">
                  <li>
                    <router-link :to="{ path: '/About_us' }">
                      <a href="#!" class="text-white">Our Vision</a>
                    </router-link>
                  </li>
                  <li>
                    <router-link :to="{ path: '/Investment_Plans' }">
                      <a href="#!" class="text-white"> testimonies</a>
                    </router-link>
                  </li>
                </ul>
              </div>
              <!--Grid column-->
            </div>
            <!--Grid row-->
          </div>
          <!-- Section: Links -->
        </div>
        <!-- Grid container -->
        <!-- INVESTMENT REGULATION container -->

        <div class="container-md">
          <div class="footer-img-sec">
            <img :src="image" alt="" srcset="" class="footer-img" />
            <img :src="image2" alt="" srcset="" class="footer-img" />
            <img :src="image3" alt="" srcset="" class="footer-img-flag" />
          </div>
        </div>
        <!-- Copyright -->
        <div class="text-center p-5 font-quicksand copyright" style="background-color: rgba(0, 0, 0, 0.2)">
          © 2023 Copyright:
          <a class="text-white" href="/Sign_up">Software Services </a>
        </div>
        <!-- Copyright -->
      </footer>
      <!-- Footer -->
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterNav',
  data() {
    return {
      image: require('@/assets/img/icon/uk2.png'),
      image2: require('@/assets/img/icon/us.png'),
      image3: require('@/assets/img/icon/uswhite.png'),
    }
  },
}
</script>

<style scoped>
.font-quicksand {
  font-family: 'Quicksand', sans-serif;
}
.link-section p {
  width: 100%;
  font-size: 15px;
  padding: 30px 0px;
  margin: 0px auto;
}

footer a {
  text-decoration: none;
}
.footer-note {
  color: #434242;
  font-size: 13px;
}
.footer-img {
  margin: 5px 10px;
  width: 30px;
}

.footer-img-flag {
  margin: 10px 10px;
  color: #434242;
  width: 50px;
}
.copyright {
  font-size: 10px;
}
/* mobile view */
@media (max-width: 886px) {
  .link-section p {
    width: 100%;
    padding: 40px 0px;
    margin: 0px;
  }

  .form-label {
    margin: 20px 0px 0px 0px;
  }
}
</style>
