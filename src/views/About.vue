<template>
  <main>
    <section class="about">
      <div class="center">
        <h2 class="texthead">Discover the fast way of delivery</h2>
      </div>

      <div class="row">
        <div class="col-1-of-2">
          <h3 class="first">one of a king state of the act</h3>
          <p class="para">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut pariatur
            nobis error quas esse iste ipsa expedita ad libero? Voluptatum
            corrupti aspernatur reprehenderit maxime dicta vitae deserunt, optio
            est quod!
          </p>
          <h3 class="first">delivery as never been so fast</h3>
          <p class="para">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut pariatur
            nobis error quas esse iste ipsa expedita ad libero? Voluptatum
            corrupti aspernatur reprehenderit maxime dicta vitae deserunt, optio
          </p>
          <button class="button2">
            <span class="tag">explore &rarr;</span>
          </button>
        </div>

        <div class="col-1-of-2">
          <div class="composition">
            <div class="tagg">
              <img
                src="../assets/mapping.jpeg"
                alt="photo 1"
                class="composition__photo composition__photo--p1"
              />
            </div>

            <img
              src="../assets/time.jpg"
              alt="photo 2"
              class="composition__photo composition__photo--p2"
            />

            <img
              src="../assets/droneme.jpeg"
              alt="photo 3"
              class="composition__photo composition__photo--p3"
            />
          </div>
        </div>
      </div>
    </section>
  </main>
  <!-- <Aboutcontent :twogrid="twogrid" /> -->
</template>

<script>
import Aboutcontent from "../views/Aboutcontent.vue";
export default {
  props: ["Aboutpage"],
};
</script>

<style lang="scss">
.about {
  margin: 10px;
  background-color: #eee;
  padding: 20rem 0 10rem 0;
  margin-top: -11.5rem !important;
  height: 55vh;
  display: fixed;

  .center {
    text-align: center;
    margin-top: -10rem;

    .texthead {
      font-size: 35px;
      text-transform: uppercase;
      font-weight: 400;
      display: inline-block;
      background-image: linear-gradient(
        to right,
        #9d455b96,
        #3f5e649c,
        #41466198
      );
      -webkit-background-clip: text;
      color: transparent;
      letter-spacing: 2px;
      transition: all 0.2s;

      &:hover {
        transform: skewY(2deg) skewX(4deg) scale(1.1);
      }
    }
  }

  @mixin clearfix {
    &::after {
      content: "";
      display: table;
      clear: both;
    }
  }

  .row {
    @include clearfix;
    max-width: 114rem;
    background-color: #eee;
    margin: 40px 80px;
    margin-bottom: 80px;

    &:not(:last-child) {
      margin-bottom: 80px;
    }

    .col-1-of-2 {
      width: calc((100% - #{60px}) / 2);
      float: left;
      &:not(:last-child) {
        margin-right: 60px;
      }
    }
    .first {
      font-size: 16px;
      display: inline-block;
      font-weight: 700;
      margin-bottom: 1rem;
      text-transform: uppercase;
    }

    .para {
      font-size: 14px;
      &:not(:last-child) {
        margin-bottom: 3rem;
      }
    }
    .button2 {
      @include clearfix;
      background-image: linear-gradient(
        to right,
        #9d455b96,
        #3f5e649c,
        #41466198
      );
      border: none;
      -webkit-background-clip: text;
      color: transparent;

      font-size: 1rem;
      text-transform: uppercase;
      display: inline-block;
      .tag {
        border-bottom: 1px solid #12ceeb81;
      }

      &:hover {
        background: linear-gradient(to right, #9d455b96, #3f5e649c, #41466198);

        color: white;
        transform: translateY(-3px);
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
        border-radius: 100px;
        text-decoration: none;
        padding: 5px 10px;
      }

      &:active {
        transform: translateY(-3px);
        box-shadow: 0 5px 10px rgba(0, 0, 0, 0.5);
      }
    }
  }
}

//second side
.composition {
  position: relative;

  &__photo {
    width: 55%;
    box-shadow: 0 1.5rem 4rem rgba(0, 0, 0, 0.4);
    border-radius: none;
    transition: transform 1s;

    position: absolute;
    outline-offset: 1rem;

    &--p1 {
      left: 0;
      top: -2rem;
    }

    &--p2 {
      right: 0;
      top: 2rem;
    }

    &--p3 {
      left: 20%;
      top: 10rem;
    }

    &:hover {
      // outline: 0.4rem solid #009cc398;
      transform: scale(1.05) translateY(-0.5rem);
      box-shadow: 0 2.5rem 4rem rgba(0, 0, 0, 0.5);
      z-index: 20;
    }
  }
  &:hover &__photo:not(:hover) {
    transform: scale(0.95);
  }
}
</style>
