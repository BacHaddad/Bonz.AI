<template>
  <header class="header">
    <nav class="header_navbar">
      <router-link to="/"> Bonz.AI </router-link>
    </nav>

    <article class="header_text">
      <h1>Bonz.AI</h1>
      <h2>An AI-Powered Eco-Stay</h2>
      <aside></aside>
    </article>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {},
};
</script>

<style scoped lang="scss">
.header {
  height: 100vh;
  width: 100vw;
  position: relative;
  background-image: linear-gradient(rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.1)), url('../assets/header-image.jpg');
  background-position: center;
  background-repeat: no-repeat;
  background-size: 110% 110%;

  &_text {
    position: absolute;
    top: 13.875rem;
    left: 10.438rem;
  }
}
</style>
