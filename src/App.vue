<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/game/darq">Darq</router-link>
      <router-link to="/game/hollow">Hollow</router-link>
      <router-link to="/game/dyson">Dyson</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style>
*{
  padding:0;
  margin:0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color:#1f003eca

}

#nav {
  display:flex;
  flex-direction: column;
  width: 5rem;
  height: 7rem;
  justify-content: space-around;
  position:fixed;
  right: 3rem;
  top:18rem;
  z-index: 100;
}

#nav a {
  text-align: left;
  font-weight: 300;
  color: #b3b3b3;
  text-decoration: none;
}

#nav a:hover{
  color:white;
}

#nav a.router-link-exact-active {
  color: #ffffff;
  font-weight: bold;
  transform: translateX(-20px);
  border-left: 5px solid #9F0098;
  padding-left: 5px
}
</style>
