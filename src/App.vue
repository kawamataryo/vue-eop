<template>
  <div id="app">
    <eop-header></eop-header>
    <div id="nav">
      <router-link to="/">Home</router-link>
      |
      <router-link to="/about">About</router-link>
      |
      <router-link to="/user">User</router-link>
    </div>
    <router-view />
  </div>
</template>
<script>
  import Header from "./components/Header";

  export default {
    components: {
      eopHeader: Header
    }
  }
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
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

h1 {
  font-size: 5rem;
}

.btn {
  cursor: pointer;
  font-weight: bold;
  font-size: 1.5rem;
  padding: 5px 30px;
  border: 1px solid #000;
  margin-left: 20px;
  &:first-child {
    margin-left: 0;
  }
}
</style>
