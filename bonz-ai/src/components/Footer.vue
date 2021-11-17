<template>
  <section class="footer">
    <div class="footer__symbols">
      <img src="..\assets\facebook.svg" alt="facebook" />
      <img src="..\assets\twitter.svg" alt="twitter" />
      <img src="..\assets\instagram.svg" alt="instagram" />
    </div>

    <p class="footer__copyright">&copy; Copyright 2021 Bonz.AI</p>
  </section>
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<style lang="scss">
.footer {
  color: $white;
  max-width: 100vw;
  overflow-x: hidden;
  @include center;
  flex-direction: column;
  background-color: $darkBrown;
  min-height: 43vh;
  padding-left: 5vw;
  padding-right: 5vw;
  margin-top: 5vh;

  &__symbols {
    > img {
      filter: invert(100%);
      height: 70px;
      width: 70px;
      border-radius: 50%;
      border: 2px solid $black inset;
      padding: 2px;
    }
    > img:hover {
      cursor: pointer;
    }
    > img:not(:first-child):not(:last-child) {
      margin: 0 41px;
    }
  }
  &__copyright {
    font-size: $fontSizeCopyright;
    margin-top: 34px;
  }
}
</style>
