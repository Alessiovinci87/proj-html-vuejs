
<template>
  <nav class="navbar">
    <div class="container">
      <div class="navbar-logo">
        <img src="/img/Logo.png" alt="Logo">
      </div>
      <ul class="nav-links">
        <li><a class="nav-link" href="#">HOME</a></li>
        <li><a class="nav-link" href="#">BLOG</a></li>
        <li class="dropdown">
          <a class="nav-link" href="#">EVENTS &#x2304;</a>
          <ul class="dropdown-content">
            <li><a href="#">CHORAL MUSIC</a></li>
            <li><a href="#">CONCERT BAND</a></li>
            <li><a href="#">OPERA CONCEERT</a></li>
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
  padding: 10px 0;
  z-index: 100; 
}

  
  .container {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  

  .navbar-logo img {
    max-width: 100px;
    height: auto;
  }
  

  .nav-links {
    display: flex;
    list-style: none;
    font-size: xx-small;
    margin: 0;
    padding: 0;
  }
  
  .nav-links li {
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
  }

  .nav-links li a.nav-link:hover {
  color: rgb(255, 106, 0);
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #030303;
  list-style: none;
  padding: 0;
  margin-top: 5px;
}

.dropdown-content li {
  padding: 10px;
}

.dropdown-content li a {
  color: white;
  text-decoration: none;
}


.dropdown:hover .dropdown-content {
  display: block;
}
  </style>
  