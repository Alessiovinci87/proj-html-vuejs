<template>
  <nav class="navbar">
    <div class="container-nav">
      <div class="navbar-logo">
        <a href=""><img src="/img/Logo.png" alt="Logo"></a>
      </div>
      <button
        class="navbar-menu-toggle"
        @click="toggleMobileMenu"
      >
        <span></span>
        <span></span>
        <span></span>
      </button>

      <div
        class="mobile-menu"
        :class="{ 'active': mobileMenuOpen }"
      >
        <ul class="mobile-nav-links">
          <li><a class="nav-link" href="#">HOME</a></li>
          <li><a class="nav-link" href="#">BLOG</a></li>
          <li class="dropdown">
            <a class="nav-link" href="#">EVENTS &#x2304;</a>
            <ul class="dropdown-content">
              <li><a href="#">CHORAL MUSIC</a></li>
              <li><a href="#">CONCERT BAND</a></li>
              <li><a href="#">OPERA CONCERT</a></li>
              <li><a href="#">SYMPHONY ORCHESTRA</a></li>
              <li><a href="#">FAMILY CONCERTS</a></li>
            </ul>
          </li>
          <li><a class="nav-link" href="#">GALLERY</a></li>
          <li><a class="nav-link" href="#">ABOUT US</a></li>
          <li><a class="nav-link" href="#">CONTACT US</a></li>
          <li class="dropdown">
            <a class="nav-link" href="#">SHOP &#x2304;</a>
            <ul class="dropdown-content">
              <li><a href="#">PRODUCT TYPE</a></li>
              <li><a href="#">SHOP PAGE</a></li>
            </ul>
          </li>
          <li><a class="nav-link" href="#"><i class="fa-solid fa-magnifying-glass search"></i></a></li>
        </ul>
      </div>
      <ul class="nav-links desktop">
        <li><a class="nav-link" href="#">HOME</a></li>
        <li><a class="nav-link" href="#">BLOG</a></li>
        <li class="dropdown">
          <a class="nav-link" href="#">EVENTS &#x2304;</a>
          <ul class="dropdown-content">
            <li><a href="#">CHORAL MUSIC</a></li>
            <li><a href="#">CONCERT BAND</a></li>
            <li><a href="#">OPERA CONCERT</a></li>
            <li><a href="#">SYMPHONY ORCHESTRA</a></li>
            <li><a href="#">FAMILY CONCERTS</a></li>
          </ul>
        </li>
        <li><a class="nav-link" href="#">GALLERY</a></li>
        <li><a class="nav-link" href="#">ABOUT US</a></li>
        <li><a class="nav-link" href="#">CONTACT US</a></li>
        <li class="dropdown">
          <a class="nav-link" href="#">SHOP &#x2304;</a>
          <ul class="dropdown-content">
            <li><a href="#">PRODUCT TYPE</a></li>
            <li><a href="#">SHOP PAGE</a></li>
          </ul>
        </li>
        <li><a class="nav-link" href="#"><i class="fa-solid fa-magnifying-glass search"></i></a></li>
      </ul>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue';

const mobileMenuOpen = ref(false);

const toggleMobileMenu = () => {
  mobileMenuOpen.value = !mobileMenuOpen.value;
};
</script>

<style lang="scss">

.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #010101;
  color: white;
  padding: 20px 0;
  z-index: 100; 
}

.navbar-logo img {
  max-width: 100px;
  height: auto;
}

.container-nav {
  margin: 0 30px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.nav-links {
  display: flex;
  align-items: center;
  list-style: none;
  font-size: small;
  margin: 0;
  padding: 0;
}

.nav-links li a {
  margin-left: 20px;
}

.nav-links li:first-child {
  margin-left: 0;
}

.nav-links li a {
  text-decoration: none;
  color: white;
  font-weight: bold;
}

.navbar-menu-toggle {
  display: none;
  cursor: pointer;
  background: none;
  border: none;
}

.navbar-menu-toggle span {
  display: block;
  width: 30px;
  height: 4px;
  background-color: white;
  margin-bottom: 6px;
}

.mobile-menu {
  display: none;
  background-color: #060606;
  position: absolute;
  top: 100%;
  left: 0;
  width: 100%;
}

.mobile-nav-links {
  display: flex;
  flex-direction: column;
  list-style: none;
  padding: 0;
  margin: 0;
}

.mobile-nav-links li {
  padding: 10px;
}

.mobile-nav-links li a {
  text-decoration: none;
  color: white;
  font-weight: bold;
}

.mobile-menu.active {
  display: block;
}

.nav-links li a.nav-link:hover {
  color: #f2870c;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #434242;
  list-style: none;
  padding: 0;
  margin-top: 5px;
}

.dropdown-content li { 
  text-align: start;
  padding: 10px;
  border-bottom: 1px solid #ffffff;
}

.dropdown-content li a {
  color: white;
  text-decoration: none;
  padding-bottom: 5px;
}

.dropdown:hover .dropdown-content {
  display: block;
}


@media (max-width: 768px) {
  .navbar-logo {
    display: none;
  }

  .nav-links {
    display: none;
  }

  .navbar-menu-toggle {
    display: block;
  }

  .navbar {
    padding: 20px;
  }

  .container-nav {
    flex-direction: column;
    align-items: center;
  }

  .navbar-menu-toggle span {
    width: 30px;
  }

  .mobile-menu {
    display: flex;
  }

  .mobile-nav-links li {
    text-align: center;
  }
}

.nav-links.desktop li {
  padding: 10px;
}


@media (min-width: 769px) {
  .nav-links.desktop {
    display: flex;
  }

  .mobile-menu {
    display: none;
  }
}
</style>
