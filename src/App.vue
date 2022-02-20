<template>
  <v-app>
    <v-app-bar>
      <!-- <router-link to="/about">About</router-link> -->
      <!-- <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
  
  </div> -->
      <v-btn color="pink  ma-2" @click="$router.push('/todoapp')">
        Todoapp</v-btn
      >
      <router-view />
      <v-content>
        <v-btn color="primary ma-2" @click="$router.push('/')"> HOME</v-btn>
        <v-btn color="accent" @click="$router.push('/about')"> About</v-btn>

        <!-- <About /> -->
      </v-content>
    </v-app-bar>
  </v-app>
</template>
<script>
// import About from "@/views/About.vue";
export default {
  name: "APP",

  components: {
    // About,
  },
};
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
