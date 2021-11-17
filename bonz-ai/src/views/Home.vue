<template>
  <section>
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

      <section class="room-type">
        <div class="room-type_image"><img src="../assets/01-night.jpg" alt="" /></div>
        <article class="room-type_text">
          <h3>Type 1</h3>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium, delectus.</p>
          <button class="button">Book</button>
        </article>
      </section>
      <section class="room-type">
        <div class="room-type_image"><img src="../assets/03-night.jpg" alt="" /></div>
        <article class="room-type_text">
          <h3>Type 2</h3>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium, delectus.</p>
          <button class="button">Book</button>
        </article>
      </section>
      <section class="room-type">
        <div class="room-type_image"><img src="../assets/07-night.jpg" alt="" /></div>
        <article class="room-type_text">
          <h3>Type 3</h3>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium, delectus.</p>
          <button class="button">Book</button>
        </article>
      </section>
      <section class="room-type">
        <div class="room-type_image"><img src="../assets/08-night.jpg" alt="" /></div>
        <article class="room-type_text">
          <h3>Type 4</h3>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium, delectus.</p>
          <button class="button">Book</button>
        </article>
      </section>
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
.header {
  .header-hero {
    position: relative;

    &_image {
      width: 100%;
      height: 70vh;
      object-fit: cover;
      box-shadow: 0 4px 4px 0 $boxShadow;
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

  p {
    margin: 51px 0;
  }
}

.rooms-type {
  margin-top: 12vh;
  @include layout-grid;
  margin-bottom: 112px;

  h2 {
    text-align: center;
    grid-column: auto / span 2;
    margin-bottom: 50px;
  }

  .room-type {
    .room-type_text {
      h3 {
        font-weight: 900;
      }
    }
  }
}

@media screen and (max-width: 900px) {
  .room-type {
    grid-column: auto / span 2;
  }
}
</style>
