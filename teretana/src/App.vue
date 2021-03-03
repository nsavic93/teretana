<template>
  <div id="app">
    <div class="nav_menu_ham" v-if="!show">
      <button class="menu_button" @click="openNav()">
        <i class="fas fa-bars"></i>
      </button>
    </div>
    <div class="nav_menu" v-if="show">
      <button class="close_button" @click="closeNav()">
        <i class="far fa-times-circle"></i>
      </button>
      <router-link to="/">Home</router-link>
      <router-link to="/about">About Us</router-link>
      <router-link to="/services">Services</router-link>
      <router-link to="/gallery">Galery</router-link>
      <router-link to="/contact">Contact</router-link>
    </div>
    <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About Us</router-link>
      <router-link to="/about">Services</router-link>
      <router-link to="/about">Galery</router-link>
      <router-link to="/about">Contact</router-link>
    </div>
    <router-view class="view" />
  </div>
</template>

<script>
// import axios from 'axios'
// import { mapActions, mapState } from "vuex";
export default {
  name: "Home",
  data() {
    return {
      show: false,
    };
  },
  methods: {
    openNav() {
      this.show = true;
    },
    closeNav() {
      this.show = false;
    },
  },
  mounted() {},
};
</script>

<style>
body {
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  justify-content: center;
}

#nav {
  padding: 30px;
  position: absolute;
  z-index: 1;
  right: 0;
  left: 0;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  /* margin-left: 10px; */
  margin-right: 32px;
  font-family: "Oswald", sans-serif;
  font-size: 15px;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 1px;
  color: white;
}
#nav a:hover {
  color: #f36100;
}

#nav a.router-link-exact-active {
  color: #f36100;
}
.view {
  position: relative;
  top: 0;
}
.nav_menu_ham {
  display: none;
}

@media only screen and (max-width: 600px) {
  #nav {
    display: none;
  }
  .nav_menu_ham {
    display: block;
    position: fixed;
    left: 10px;
    top: 10px;
    z-index: 3;
  }
  .menu_button {
    background: none;
    color: white;
    border: none;
    z-index: 4;
    font-size: 40px;
  }
  .menu_button:active {
    outline: none;
  }
  .menu_button:focus {
    outline: none;
  }
  .close_button {
    background: none;
    color: white;
    border: none;
    position: absolute;
    right: 10px;
    top: 10px;
    font-size: 20px;
  }
  .nav_menu {
    z-index: 3;
    position: fixed;
    left: 0;
    background-color: #21252999;
    width: 50%;
    height: 100vh;
    padding: 30px;
    display: flex;
    flex-direction: column;
  }
  .nav_menu a {
    margin-top: 10px;
    font-weight: bold;
    color: #2c3e50;
    font-family: "Oswald", sans-serif;
    font-size: 15px;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 1px;
    color: white;
  }
}
</style>
