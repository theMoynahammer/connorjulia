<template>
  <div id="app">
    <!-- <div id="mainModal"> -->
     <div id="nav">
       <router-link to="/">Wedding Info</router-link> |
       <router-link to="/about">About Us</router-link> |
       <router-link to="/connor">Connor</router-link> |
       <router-link to="/julia">Julia</router-link>
      <!-- </div> -->
      <div id='wrapper'>
      <router-view/>
      </div>
    </div>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: white;
  width: 350px;
  height: 400px;
}

#wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  height:325px;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  font-size: 15px;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: rgb(20, 130, 220);
}
</style>
