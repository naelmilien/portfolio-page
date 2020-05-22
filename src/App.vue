<template>
  <div id="app">
    <div id="nav">
      <div id="logo">
        <!-- <img src="./assets/profile-pic.jpeg" alt /> -->
        <p>nathanael milien</p>
      </div>
      <div id="router-links">
        <router-link to="/">Home</router-link>|
        <router-link to="/about">About</router-link>|
        <router-link to="/projects">Projects</router-link>|
        <router-link to="/contact">Contact me</router-link>
      </div>
    </div>
    <router-view />
  </div>
</template>

<style>
#app {
  /* font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center; */
  color: #2c3e50;
}

/* #logo {
  display: flex;
  flex-direction: row;
} */

#logo p {
  font-family: "Parisienne", cursive;
  margin: 0px;
  font-size: 40px;
}

#nav {
  /* padding: 30px; */
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  /* border-bottom: 1px solid #2c3e50; */
  color: #2c3e50;
  box-sizing: border;
  font-family: "Balsamiq sans", cursive;
}

#router-links {
  padding: 20px;
}

#nav a {
  font-weight: bold;
  margin: 15px;
  color: #2c3e50;
  text-decoration: none;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

@media screen and (max-width: 780px) {
  #nav {
    flex-direction: column;
    text-align: center;
    margin: 0;
    padding: 0;
  }

  #router-links {
    padding: 5px;
  }

  #nav a {
    margin: 5px;
  }
}
</style>
