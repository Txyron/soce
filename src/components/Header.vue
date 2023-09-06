<template>
  <div id="app">
    <header>
      <nav class="navbar">
        <div class="logo">
          <img src="../assets/img/Logo1.png" alt="">
        </div>

        <div class="menu-toggle" @click="menuOuvert = !menuOuvert" :class="{ ouvert: menuOuvert, ferme: !menuOuvert }">
          <span></span>
          <span></span>
          <span></span>
        </div>
        <ul class="nav-links">
          <li><router-link to="/">Accueil</router-link></li>
          <li><router-link to="/about">Avis de passage</router-link></li> 
          <li><router-link to="/contact">Contact</router-link></li>
        </ul>
        <div class="logomini">
          <img src="../assets/img/Logo2.png" alt="">
        </div>
      </nav>
    </header>
  </div>
</template>


<script>

export default {
  data() {
    return {
      menuOuvert: false,
    };
  },
  methods: {
    toggleMenu() {
      this.menuOuvert = !this.menuOuvert;
    },
  },
};
</script>


  <style scoped>

  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 25px;
    background-color: #3d3d33;
    color: #ffffff;
    border-radius: 0 0 20px 20px;
  }
  
  .logo img {
    height: 40px;
  }
  
  .logomini img {
    height: 50px;
  }
  
  .menu-toggle {
    display: none;
    flex-direction: column;
    cursor: pointer;
  }
  
  .menu-toggle span {
    width: 25px;
    height: 3px;
    background-color: #fff;
    margin: 3px 0;
  }
  
  .nav-links {
    list-style: none;
    display: flex;
    margin: 0;
    padding: 0;
  }
  
  .nav-links li {
    margin-right: 20px;
  }
  
  .nav-links a {
    color: #ffffff;
    text-decoration: none;
    position: relative;
    font-size: 16px;
  }
  
  .nav-links a::before {
    content: '';
    position: absolute;
    bottom: -2px;
    left: 0;
    width: 0;
    height: 2px;
    background-color: #55ab41;
    transition: width 0.5s ease;
  }
  
  .nav-links a:hover::before {
    width: 100%;
  }
  
  @media screen and (max-width: 768px) {
    .navbar {
      flex-direction: column;
      align-items: flex-start;
    }
  
    .menu-toggle {
      display: flex;
      margin-bottom: 10px;
    }
  
    .nav-links {
      flex-direction: column;
    }
  
    .nav-links li {
      margin-right: 0;
      margin-bottom: 10px;
    }
  }
  </style>
  