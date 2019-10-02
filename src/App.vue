<template>
  <div id="app">
    <div id="nav">
          <router-link id="monday-nav" to="/">Monday  </router-link>
          <router-link id="tuesday-nav" to="/tuesday">Tuesday  </router-link>
          <router-link id="wednesday-nav" to="/wednesday">Wednesday  </router-link>
          <router-link id="thursday-nav" to="/thursday">Thursday  </router-link>
          <router-link id="friday-nav" to="/friday">Friday  </router-link>
          <router-link id="saturday-nav" to="/saturday">Saturday  </router-link>
          <router-link id="sunday-nav" to="/sunday">Sunday  </router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
