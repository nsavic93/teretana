<template>
  <div id="app">
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

<style>
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
</style>
