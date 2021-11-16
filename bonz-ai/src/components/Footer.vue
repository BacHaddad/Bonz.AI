<template>
  <section class="footer">
    <img src="..\assets\footer-icons.svg" alt="" />
  </section>
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style lang="scss">
.footer {
  max-width: 100vw;
  overflow-x: hidden;
  @include center;
  background-color: $darkBrown;
  min-height: 43vh;
  padding-left: 5vw;
  padding-right: 5vw;
}
</style>
