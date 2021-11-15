<template>
  <nav class="navbar">
    <router-link class="brand" to="/"> <img src="..\assets\bonzai-logo.png" alt="" /> </router-link>
    <router-link class="link" to="/"> About </router-link>
    <router-link class="link" to="/"> Stay </router-link>
    <button class="button">Book</button>
  </nav>
</template>

<script>
export default {
  name: 'Header',
};
</script>

<style lang="scss">
.navbar {
  width: 100%;
  @include center;
  background-color: $greenBlue;
  height: 15vh;
  padding-left: 5vw;
  padding-right: 5vw;
  border-bottom: 11px solid $neonBlue;

  & > .brand {
    margin-right: auto;
  }
}
</style>
