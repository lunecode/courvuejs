<template>
  <div id="app">
    <!-- <FirstComponent/>
    <Second/>
    <Third/>
    <Fourth/>
    <Firth/> -->
    <Navbar/>
    <div id="nav">
      <!-- <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
      <router-link to="/test">Test</router-link> -->
    </div>
    <router-view/>
  </div>
</template>

<script>

import Navbar from './components/Navbar'

import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
// app.js
import Vue from 'vue'
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'

// Install BootstrapVue
Vue.use(BootstrapVue)
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin)



// import FirstComponent from './components/FirstComponent'
// import Second from './components/Second'
// import Third from './components/Third'
// import Fourth from './components/Fourth'
// import Firth from './components/Firth'

export default {
  name: 'App',
  components: {
    // FirstComponent,
    // Second,
    // Third,
    // Fourth,
    // Firth,
    Navbar
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
