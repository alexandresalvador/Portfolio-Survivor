<template>
  <div id="app">
    <navbar>
    </navbar>
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/educacao">Educacao</router-link> |
      <router-link to="/trabalho">Jobs</router-link> |
      <router-link to="/contato">Contato</router-link> |
    </nav>
    <router-view/>
  </div>

</template>
<script>
import navbar from '@/components/Navbar.vue';

export default {
  components: {
    navbar,
  },
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
