<template>
<div class="container">
<NavBar/>
<DevelopStore />
<AllInOnePlace />
<SpecialApps />
  <router-view/>
  </div>
</template>

<script>
import NavBar from './views/NavBar.vue'
import DevelopStore from './views/DevelopStore.vue'
import AllInOnePlace from './views/AllInOnePlace.vue'
import SpecialApps from './views/SpecialApps.vue'
export default {
  name:'App',
  components:{
    NavBar,
    DevelopStore,
    AllInOnePlace,
    SpecialApps,
  }
}
</script>
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
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
