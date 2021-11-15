<template>
  <footer class="footer">
    <img src="../assets/foter-icons.svg" alt="" />
  </footer>
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style lang="scss">
.footer {
  width: 100%;
  @include center;
  background-color: $darkBrown;
  height: 43vh;
  padding-left: 5vw;
  padding-right: 5vw;
}
</style>
