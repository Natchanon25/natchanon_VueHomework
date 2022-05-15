<template>
  <div id="app">
    <router-link class="link" :to="{ path: '/' }">Profile</router-link>
    <router-link class="link" :to="{ path: '/contact' }">Contact</router-link>
    <router-view />
  </div>
</template>

<script>
export default {
  name: "App",
};
</script>

<style>
html,
body {
  background-color: rgb(188, 240, 175);
}
#app {
  margin: 60px;
  text-align: left;
}
.link {
  display: inline-block;
  padding: 10px;
  text-decoration: none;
  color: inherit;
}
.router-link-exact-active {
  color: blue;
}
</style>

