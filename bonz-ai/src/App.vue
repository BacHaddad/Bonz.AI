<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style lang="scss">
*,
body,
html {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
#app {
  max-width: 1440px;
  margin: 0 auto;
}

@media screen and (max-width: $breakPoint0) {
  #app {
    max-width: 100vw;
  }
}
</style>
