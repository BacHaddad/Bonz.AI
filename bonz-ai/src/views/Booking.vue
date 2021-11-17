<template>
  <div>
    <Navbar />
    <section class="booking-info">
      <h2>Booking</h2>
      <article class="booking-info_details">
        <div>
          <p>Check-in dates</p>
          <p>Dec 22</p>
        </div>
        <img src="../assets/checkin-dates.svg" alt="" />
        <div class="border"></div>
        <div>
          <p>Check-in dates</p>
          <p>Dec 22</p>
        </div>
        <img src="../assets/checkin-dates.svg" alt="" />
        <div class="border"></div>
        <div>
          <p>Check-in dates</p>
          <p>Dec 22</p>
        </div>
        <img src="../assets/guests.svg" alt="" />
        <div class="border"></div>
        <div>
          <p>Check-in dates</p>
          <p>Dec 22</p>
        </div>
        <img src="../assets/rooms.svg" alt="" />
      </article>
    </section>
    <hr />

    <article class="room-booking">
      <section class="room-booking__type">
        <div class="image"><img src="../assets/01-night.jpg" alt="Room img" /></div>
        <article class="text">
          <h3>Room Type 1</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </article>
      </section>
      <section class="room-booking__details">
        <article class="input">
          <p class="drone">
            On-demand drone-delivered coffee <br />
            <strong>100 SEK</strong>
          </p>
          <input class="checkbox-round" type="checkbox" name="coffee" checked />
        </article>
        <article class="input">
          <p>
            On-demand drone-delivered food <br />
            <strong>200 SEK</strong>
          </p>
          <input class="checkbox-round" type="checkbox" name="food" />
        </article>
        <p>Total 1100 SEK</p>
        <button class="button">Book</button>
      </section>
    </article>

    <hr />

    <article class="room-booking">
      <section class="room-booking__type">
        <div class="image"><img src="../assets/07-night.jpg" alt="Room img" /></div>
        <article class="text">
          <h3>Room Type 2</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </article>
      </section>
      <section class="room-booking__details">
        <article class="input">
          <p class="drone">
            On-demand drone-delivered coffee <br />
            <strong>100 SEK</strong>
          </p>
          <input class="checkbox-round" type="checkbox" name="coffee" />
        </article>
        <article class="input">
          <p>
            On-demand drone-delivered food <br />
            <strong>200 SEK</strong>
          </p>
          <input class="checkbox-round" type="checkbox" name="food" />
        </article>
        <p>Total 1000 SEK</p>
        <button class="button">Book</button>
      </section>
    </article>

    <hr />

    <article class="room-booking">
      <section class="room-booking__type">
        <div class="image"><img src="../assets/03-night.jpg" alt="Room img" /></div>
        <article class="text">
          <h3>Room Type 3</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </article>
      </section>
      <section class="room-booking__details">
        <article class="input">
          <p class="drone">
            On-demand drone-delivered coffee <br />
            <strong>100 SEK</strong>
          </p>
          <input class="checkbox-round" type="checkbox" name="coffee" />
        </article>
        <article class="input">
          <p>
            On-demand drone-delivered food <br />
            <strong>200 SEK</strong>
          </p>
          <input class="checkbox-round" type="checkbox" name="food" />
        </article>
        <p>Total 1000 SEK</p>
        <button class="button">Book</button>
      </section>
    </article>

    <hr />

    <article class="room-booking">
      <section class="room-booking__type">
        <div class="image"><img src="../assets/08-night.jpg" alt="Room img" /></div>
        <article class="text">
          <h3>Room Type 4</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </article>
      </section>
      <section class="room-booking__details">
        <article class="input">
          <p class="drone">
            On-demand drone-delivered coffee <br />
            <strong>100 SEK</strong>
          </p>
          <input class="checkbox-round" type="checkbox" name="coffee" />
        </article>
        <article class="input">
          <p>
            On-demand drone-delivered food <br />
            <strong>200 SEK</strong>
          </p>
          <input class="checkbox-round" type="checkbox" name="food" />
        </article>
        <p>Total 1000 SEK</p>
        <button class="button">Book</button>
      </section>
    </article>

    <hr />
    <article class="booking-review">
      <h2>Your Booking</h2>
      <section>
        <p>Wed, Dec 22, 2021 - Sun, Dec 26, 2021</p>
        <p>1 Adult</p>
        <p>4 nights</p>
        <p>Room Type 2</p>
        <p>Drone-delivered coffee included</p>
      </section>
      <section>
        <img src="../assets/07-night.jpg" alt="" />
        <p>Total 1100 SEK</p>
      </section>
      <button class="button">Complete your booking</button>
    </article>
    <Footer />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'Booking',
  components: { Navbar, Footer },
};
</script>

<style lang="scss">
.booking-info {
  margin: 4rem 0;
  padding: 0 2rem;
  &_details {
    padding: 1em;
    width: 100%;
    p {
      font-size: $fontSizeCopyright;
    }
    > img {
      width: 50px;
      height: 50px;
    }
    > img:hover {
      cursor: pointer;
    }
  }
}

.room-booking {
  height: 25rem;
  width: 100%;
  @include center;
  padding: 0 5vw;

  &__type {
    flex-basis: 60%;
    display: flex;

    .image {
      flex-basis: 60%;
      margin-right: 4%;
      > img {
        object-fit: cover;
        width: 100%;
      }
    }

    .text {
      flex-basis: 40%;

      p {
        font-size: 1.25rem;
        line-height: 100%;
        margin: 8% 0;
      }
    }
  }

  &__details {
    flex-basis: 40%;
    @include center;
    flex-direction: column;
    align-items: flex-end;
    text-align: right;
    .input {
      @include center;
      margin: 3% 0;
    }
    & .input > p {
      font-size: 1.25rem;
      margin: 5px;
      line-height: 100%;
    }
    > p {
      font-size: 1.25rem;
      font-weight: bold;
      margin-bottom: 2%;
    }
  }
}

.booking-review {
  width: 62rem;
  height: 48rem;
  background-color: $lightGrey;
  box-shadow: 0 4px 4px 0 $boxShadow;
  @include layout-grid;
  margin: 50px auto;
  gap: 0 8rem;
  h2 {
    grid-column: auto / span 2;

    align-self: center;
    justify-self: center;
    margin: 60px 0;
  }
  img {
    width: 250px;
    margin-bottom: 8%;
  }
  p {
    font-size: 1.2rem;
    margin-bottom: 8px;
  }
  .button {
    grid-column: auto / span 2;
    align-self: center;
    justify-self: center;
  }
}
</style>
