<template>
  <section class="wrapper">
    <Header />
  </section>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue';

export default {
  name: 'Home',
  components: {
    Header,
  },
};
</script>

<style lang="scss">
.wrapper {
  max-width: 1440px;
  height: 100vh;
  margin: 0 auto;
}
</style>
