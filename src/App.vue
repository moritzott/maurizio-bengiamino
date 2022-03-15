<template>
<!-- the header -->
  <header>
    <div class="header-container">
      <!-- Name of the App -->
      <span class="name-of-app">Maurizio Bengiamino</span>
      <!-- Burger Menu -->
      <span @click="openMobileNavbar" class="burger-menu-sign">&#9776;</span>
      <!-- Navbar -->
      <NavbarDesktop />
      <!-- Mobile Navbar as Modal -->
      <MobileNavbarModal>
        <NavbarMobile />
      </MobileNavbarModal>
    </div>
  </header>

  <!-- The specific Content of the page(s) -->
  <ContentContainer />
  

</template>

<script>
import NavbarDesktop from '@/components/NavbarDesktop.vue'
import NavbarMobile from '@/components/NavbarMobile.vue'
import MobileNavbarModal from '@/components/MobileNavbarModal.vue'
import ContentContainer from '@/components/ContentContainer.vue'

export default {
  components: {
    NavbarDesktop,
    NavbarMobile,
    MobileNavbarModal,
    ContentContainer
  },
  methods: {
    openMobileNavbar () {
      const navbarModal = document.querySelector('.modal-navbar');
        navbarModal.style.display = 'block';
      }
    }
  }

</script>

<style>
/* #app {

}

nav {

} */

/* Import the Fonts css file */
@import './assets/css/fonts.css';

/* Import the global css file */
@import './assets/css/global.css';

nav a {
  text-decoration: none;
  color: black;
  text-transform: uppercase;
}

nav a.router-link-exact-active {
  border-bottom: 2px solid black;
}

@media only screen and (max-width: 952px) {
      nav a.router-link-exact-active {
          border: none;
      }

      nav a.router-link-exact-active span{
          border-bottom: 2px solid black;
      }
  }
</style>
