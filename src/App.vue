<template>
  <router-link :to="{ name: 'Landing' }"></router-link>
  <router-link :to="{ name: 'About' }"></router-link>
  <router-view />
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
