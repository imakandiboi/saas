<template>
  <div>
    <nav class="navbar navbar-light navbar-expand-lg bg-light py-2 py-sm-3 px-2 fixed-top">
      <div class="container">
        <router-link :to="{ path: '/' }">
          <img :src="image" alt="" srcset="" class="nav-img" />
          <a class="navbar-brand font-quicksand" href="/"> <img src="" alt="" srcset="" class="logo" /> Software Services </a>
        </router-link>
        <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="offcanvas side-bar offcanvas-end font-quicksand" id="offcanvasNavbar" tabindex="-1" aria-labelledby="offcanvasNavbarLabel">
          <div class="offcanvas-header">
            <img src="" alt="" srcset="" class="logo" />
            <button type="button" class="btn-close text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
          </div>
          <div class="offcanvas-body">
            <ul class="navbar-nav justify-content-end flex-grow-1 p-2">
              <li class="nav-item">
                <router-link :to="{ path: '/' }">
                  <span class="d-flex align-items-center gap-3">
                    <a class="nav-link active" aria-current="page" href="/">Home</a>
                  </span>
                </router-link>
              </li>
              <li class="nav-item">
                <router-link :to="{ path: '/' }">
                  <span class="d-flex align-items-center gap-3">
                    <a class="nav-link" href="/">About Us</a>
                  </span>
                </router-link>
              </li>
              <li class="nav-item">
                <router-link :to="{ path: '/' }">
                  <span class="d-flex align-items-center gap-3">
                    <a class="nav-link" href="/">Investment Plan</a>
                  </span>
                </router-link>
              </li>

              <!-- USER PROFILE SECTION -->
              <!-- <li v-if="!isAuthenticated && !isLoading" class="nav-item gap-2">
                <button id="qsLoginBtn" class="btn btn-margin" @click.prevent="login">Login / Sign Up</button>
              </li> -->

              <!-- if login is verified it displays the user  -->
              <!-- 
              <div class="nav-item d-flex gap-2 auth" v-if="isAuthenticated">
                <a class="nav-link d-flex" href="#">
                  <img :src="user.picture" alt="User's profile picture" class="nav-user-profile rounded-circle d-flex" width="27" />
                </a>
                <li class="nav-item d-flex gap-2 auth">
                  <div class="d-flex">{{ user.name }}</div>
                  <router-link to="/profile" class="d-flex"> <font-awesome-icon class="mr-3" icon="user" />Profile </router-link>
                  <a id="qsLogoutBtn" href="#" class="d-flex" @click.prevent="logout"> <font-awesome-icon class="mr-3" icon="power-off" />Log out </a>
                </li>
              </div> -->

              <!-- USER PROFILE SECTION -->
            </ul>
          </div>
        </div>
      </div>
    </nav>
    <!-- this is news  -->

    <div class="mt-5 widget fixed container-fluid">
      <div id="coinmarketcap-widget-marquee" coins="1,1027,825,2010,6636,1883,11346,1831" currency="USD" theme="light" transparent="false" show-symbol-logo="true"></div>
    </div>
    <!-- END OF NAVIGATION BAR -->
  </div>
</template>

<script>
// import { useAuth0 } from '@auth0/auth0-vue'

export default {
  name: 'NavBar',
  data() {
    return {
      image: require('@/assets/img/bitcoin.png'),
      loading: Boolean,
    }
  },

  // setup() {
  //   const auth0 = useAuth0()

  //   return {
  //     isAuthenticated: auth0.isAuthenticated,
  //     isLoading: auth0.isLoading,
  //     user: auth0.user,
  //     login() {
  //       auth0.loginWithRedirect()
  //     },
  //     logout() {
  //       auth0.logout({
  //         returnTo: window.location.origin,
  //       })
  //     },
  //   }
  // },
}
</script>

<style scoped>
.font-quicksand {
  font-family: 'Quicksand', sans-serif;
}
.navbar-toggler {
  outline: none;
}
.auth {
  padding: 2px 0px;
}
.widget {
  padding: 0px;
  position: absolute;
  top: 4%;
  z-index: 3;
}
.nav-img {
  width: 30px;
}
.headnav {
  height: 70px;
}
.btn-sign {
  margin: 0px 20px;
  width: 90px;
}
.headnav a {
  font-family: Snippet;
  font-size: 15px;
  font-style: normal;
  font-variant: small-caps;
  font-weight: 100;
}
.navbar a {
  text-decoration: none;
}
@media (max-width: 886px) {
  .widget {
    padding: 0px;
    position: absolute;
    top: 0.8%;
    z-index: 3;
  }
  .auth {
    padding: 0px;
  }
}
</style>
