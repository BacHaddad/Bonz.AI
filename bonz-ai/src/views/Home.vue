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
    <article class="rooms-type">
      <h2>Select your stay</h2>
      <div class="rooms">
        <section class="room-type">
          <img class="room-type_image" src="..\assets\01-night.jpg" alt="" />
          <article class="room-type_text">
            <h3>Type 1</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio tempora officia eos asperiores itaque a rem veniam ex mollitia esse.</p>
            <button class="button">Book</button>
          </article>
        </section>
        <section class="room-type">
          <img class="room-type_image" src="..\assets\03-night.jpg" alt="" />
          <article class="room-type_text">
            <h3>Type 2</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio tempora officia eos asperiores itaque a rem veniam ex mollitia esse.</p>
            <button class="button">Book</button>
          </article>
        </section>
        <section class="room-type">
          <img class="room-type_image" src="..\assets\07-night.jpg" alt="" />
          <article class="room-type_text">
            <h3>Type 3</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio tempora officia eos asperiores itaque a rem veniam ex mollitia esse.</p>
            <button class="button">Book</button>
          </article>
        </section>
        <section class="room-type">
          <img class="room-type_image" src="..\assets\08-night.jpg" alt="" />
          <article class="room-type_text">
            <h3>Type 4</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio tempora officia eos asperiores itaque a rem veniam ex mollitia esse.</p>
            <button class="button">Book</button>
          </article>
        </section>
      </div>
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
    min-height: 70vh;
    padding: 130px;
    @include center;
    flex-flow: column wrap;
  }

  .rooms-type {
    margin-top: 12vh;
    h2 {
      text-align: center;
    }

    .room-type {
      min-height: 23vh;

      .room-type_image {
        object-fit: cover;
        flex-basis: 60%;
      }
      .room-type_text {
        flex-basis: 40%;
      }
    }
  }
}
</style>
