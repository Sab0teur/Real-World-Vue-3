<template>
  <div id="app">
    <div id="nav">
      <router-link to="/home">Home</router-link>&nbsp;|
      <router-link :to="{ name: 'EventList' }">Events</router-link>&nbsp;|
      <router-link to="/about">About</router-link>
    </div>
    <h1 id="title">Basswave</h1>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#title {
  /* font-weight: bold; */
  font-size: 50px;
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

h4 {
  font-size: 20px;
}
</style>
