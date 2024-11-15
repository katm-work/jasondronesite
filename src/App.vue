<template>
  <div class="header-container">
    <div>
      <Logo altText="My Company Logo" logoClass="custom-logo" />
    </div>
    <div class="company-name">
      <h1>Jason's Drone Services</h1>
    </div>
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link :to="{ name: 'services' }">Services</router-link> |
      <router-link :to="{ name: 'contacts' }">Contact Us</router-link>
    </nav>
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
.company-name {
  display: flex;
  max-width: auto;
  text-align: center;
  align-items: center;
  margin: auto;
}

.header-container {
  display: flex;
  max-width: auto;
  margin: auto;
  flex-direction: row;
  text-align: center;
  justify-content: space-between;
  align-content: center;
}

.custom-logo {
  display: flex;
  max-width: 150px;
  margin: 15%;
  border-radius: 40%;
  border: 5px solid #2c3e50;
  background-size: contain;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #3C896D;
  background-size: cover;
  overflow: hidden;
}


nav {
  padding: 1%;
  margin: auto;
  background-color: #3C896D;
  border-radius: 45px;
}

nav a {
  font-size: larger;
  font-weight: bold;
  color: #2c3e50;

}

nav a.router-link-exact-active {
  color: #EDF2F4;
  background-color: #2c3e50;
}
</style>
