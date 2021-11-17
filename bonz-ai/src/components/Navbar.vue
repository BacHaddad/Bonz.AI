<template>
  <nav class="navbar">
    <router-link v-on:click="goToHome" class="brand" to="/"> <img src="..\assets\logo.svg" alt="" /> </router-link>
    <router-link class="link" to="/"> About </router-link>
    <router-link class="link" to="/"> Stay </router-link>
    <button v-on:click="goToBooking" class="button">Book</button>
    <div class="hamburger">&#9776;</div>
  </nav>
</template>

<script>
export default {
  name: 'Header',
  methods: {
    goToHome: function () {
      this.$router.push('/');
    },
    goToBooking: function () {
      this.$router.push('/booking');
    },
  },
};
</script>

<style lang="scss">
.navbar {
  max-width: 100vw;
  @include center;
  background-color: $greenBlue;
  min-height: 15vh;
  padding-left: 5vw;
  padding-right: 5vw;
  border-bottom: 11px solid $neonBlue;

  & > .brand {
    margin-right: auto;
  }
  .hamburger {
    display: none;
    font-size: 3rem;
    line-height: 150%;
  }
}

@media screen and (max-width: 700px) {
  .navbar > .button,
  .link {
    display: none;
  }
  .navbar > .hamburger {
    display: inline-block;
  }
}
</style>
