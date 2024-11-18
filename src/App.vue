<template>
  <div>
    <div id="header-container">
      <Logo altText="My Company Logo" logoClass="custom-logo" />
      <h1><b>Jason's Drone Services</b></h1>
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link :to="{ name: 'services' }">Services</router-link> |
      <router-link :to="{ name: 'contacts' }">Contact Us</router-link>
    </nav>
    </div>
  </div>
  <router-view />
</template>

<script>
import Logo from './components/Logo.vue';

export default {
  components: {
    Logo
  }
};
</script>

<style>
#header-container {
  display: flex;
  width: 100%;
  margin: auto;
  flex-direction: row;
  justify-content: space-between;
  align-content: center;
  background-color:#8AA8A1;
  border-bottom: 5px solid white;
}

.custom-logo {
  display: flex;
  max-width: 200px;
  max-height: 120px;
  margin: 20px auto 30px 50px;
  border-radius: 40%;
  border: 5px solid #2c3e50;
}

#app {
  font-family: "Host Grotesk", sans-serif;
  font-optical-sizing: auto;
  font-weight: 400;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #EDF2F4;
  background-color: #2c3e50;
  background-size: cover;
  text-shadow: 2px 2px #0A100DA3;
}


nav {
  margin: auto;
  border-radius: 45px;
  text-shadow: -1px -1px #0A100DA3;
  
}

nav a {
  font-size: larger;
  font-weight: bold;
  color: #EDF2F4;
  transition:ease-in background-color 0.3s;

}
nav a:hover {
  color: #2c3e50;
  }

nav a.router-link-exact-active {
  color: #EDF2F4;
  background-color: #2c3e50;
  padding: 0 5px;
  border: 2px;
  border-radius: 5px;
  
}
</style>
