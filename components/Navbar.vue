<template>
  <div>
    <b-navbar
      toggleable="lg"
      type="light"
      variant="white"
      class="shadow padding-navbar"
    >
      <nuxt-link to="/">
        <img src="logo.svg" alt="" srcset="" />
      </nuxt-link>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#"
            ><nuxt-link to="/">Beranda</nuxt-link></b-nav-item
          >
          <b-nav-item href="#"
            ><nuxt-link to="/product">Produk</nuxt-link></b-nav-item
          >
          <b-nav-item href="#"
            ><nuxt-link to="/promo">Promo</nuxt-link></b-nav-item
          >
          <b-nav-item href="#"
            ><nuxt-link to="/about-us">Tentang Kami</nuxt-link></b-nav-item
          >
          <b-nav-item href="#"
            ><nuxt-link to="contact">Hubungi Kami</nuxt-link></b-nav-item
          >
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item href="#"
            ><i class="fa-solid fa-cart-shopping"></i
          ></b-nav-item>
          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template #button-content>
              <em>User</em>
            </template>
            <b-dropdown-item href="#">Profile</b-dropdown-item>
            <b-dropdown-item href="#">Sign Out</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>
<style scoped>
  a{
    color: black;
    text-decoration: none;
  }
</style>
