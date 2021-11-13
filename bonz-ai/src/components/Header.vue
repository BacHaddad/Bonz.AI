<template>
  <header class="header">
    <nav class="header_navbar">
      <router-link to="/"> Bonz.AI </router-link>
    </nav>

    <article class="header_text">
      <h1>Bonz.AI</h1>
      <p>An AI-Powered Eco-Stay</p>
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

<style lang="scss">
@import '@/sass/_variables.scss';
@import '@/sass/_mixins.scss';
@import '@/sass/_typography.scss';
.header {
  height: 100%;
  width: 100%;

  background-image: linear-gradient(rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.1)), url('../assets/header-image.jpg');
  background-position: center center;
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: cover;

  &_text {
    color: $white;
    width: fit-content;
    margin-top: 20%;
    margin-left: 15%;
    text-align: center;
    p {
      margin: 1.6rem 0;
      font-size: $fontSizeHeroText;
    }

    aside {
      height: 5px;
      width: 100%;
      transform: scale(1.25);
      transform-origin: center;
      background-color: $neonBlue;
    }
  }
}
</style>
