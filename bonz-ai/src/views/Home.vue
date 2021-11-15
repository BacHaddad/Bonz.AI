<template>
  <section class="wrapper">
    <Navbar />
    <header class="header">
      <article class="header-hero">
        <img class="header-hero_image" src="..\assets\02-night.jpg" alt="" />
        <section class="header-hero_content">
          <h1>Bonz.AI</h1>
          <p>An AI-Powered Eco-Stay</p>
          <aside></aside>
        </section>
      </article>
    </header>
    <article class="about">
      <h2>Bonz.AI</h2>
      <p>Hello from Bonz.AI 👋 we are thrilled to welcome you to our AI-powered eco-stay at Bohuslän to the north of Gothenburg, Sweden. We believe in offering a personalized stay like none other, by bringing the ultimate contact-less experience to you at your finger tips - on your mobile device. Sit back, relax and let Bonz.AI take care of you.</p>
      <button class="button">Book Now</button>
    </article>
    <Footer />
  </section>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'Home',
  components: {
    Navbar,
    Footer,
  },
};
</script>

<style lang="scss">
.wrapper {
  max-width: 1440px;
  margin: 0 auto;

  .header {
    .header-hero {
      position: relative;

      &_image {
        width: 100%;
        height: 70vh;
        object-fit: cover;
        box-shadow: 0 4px 4px 0 rgba(0, 0, 0, 0.25);
      }

      &_content {
        position: absolute;
        top: 10vh;
        left: 10vw;

        h1 {
          color: $greenBlue;
          text-align: center;
        }
        p {
          color: $white;
        }

        aside {
          background-color: $neonBlue;
          height: 4px;
          transform: scale(1.2);
          margin-top: 3vh;
        }
      }
    }
  }

  .about {
    background-color: $lightGrey;
    height: 70vh;
    padding: 130px;
    @include center;
    flex-flow: column wrap;
    justify-content: space-between;
  }
}
</style>
