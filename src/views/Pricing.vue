<template>
  <section class="section-tours">
    <div class="center">
      <h2 class="texthead">our sector</h2>
    </div>
    <div class="rowl">
      <div class="col-1-of-3">
        <div class="card">
          <div class="card__side card__side--front">
            <div class="card__picture card__picture--1"></div>
            <h4 class="card__heading--1">
              <span class="card__span card__span--1"> tracking made easy </span>
            </h4>
            <div class="card__details--1">
              <ul>
                <li>7 times a week</li>
                <li>3 hours flight time</li>
                <li>5 login access</li>
                <li>survey and detect</li>
                <li>Difficulty; easy</li>
              </ul>
            </div>
          </div>
          <div class="card__side card__side--back card__side--back-1">
            <div class="card__cta">
              <div class="card__price-box">
                <p class="card__price-only card__price-only--1">Only</p>
                <p class="card__price-value">$200</p>
              </div>
              <button class="point">
                <span class="point__1">Subscribe !</span>
              </button>
            </div>
          </div>
        </div>
      </div>

      <div class="col-1-of-3">
        <div class="card">
          <div class="card__side card__side--front">
            <div class="card__picture card__picture--2"></div>
            <h4 class="card__heading--2">
              <span class="card__span card__span--2">
                medical delivery made easy
              </span>
            </h4>
            <div class="card__details--2">
              <ul>
                <li>7 times a week</li>
                <li>3 hours flight time</li>
                <li>5 login access</li>
                <li>survey and detect</li>
                <li>Difficulty; easy</li>
              </ul>
            </div>
          </div>
          <div class="card__side card__side--back card__side--back-2">
            <div class="card__cta">
              <div class="card__price-box">
                <p class="card__price-only card__price-only--2">Only</p>
                <p class="card__price-value">$300</p>
              </div>
              <button class="point">
                <span class="point__2">Subscribe !</span>
              </button>
            </div>
          </div>
        </div>
      </div>

      <div class="col-1-of-3">
        <div class="card">
          <div class="card__side card__side--front">
            <div class="card__picture card__picture--3"></div>
            <h4 class="card__heading--3">
              <span class="card__span card__span--3">
                delivery has never been so fast
              </span>
            </h4>
            <div class="card__details--3">
              <ul>
                <li>7 times a week</li>
                <li>3 hours flight time</li>
                <li>5 login access</li>
                <li>survey and detect</li>
                <li>Difficulty; easy</li>
              </ul>
            </div>
          </div>
          <div class="card__side card__side--back card__side--back-3">
            <div class="card__cta">
              <div class="card__price-box">
                <p class="card__price-only card__price-only--3">Only</p>
                <p class="card__price-value">$100</p>
              </div>
              <button class="point">
                <span class="point__3">Subscribe !</span>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="center2">
      <button class="last1">
        <span class="lastt"> Discover all sectors </span>
      </button>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss">
.section-tours {
  background-color: #eee;
  padding: 9rem 0 9rem 0;
  margin: 10px;
  margin-top: -7rem;
  .center {
    text-align: center;

    .texthead {
      margin-top: -5rem;
      font-size: 35px;
      text-transform: uppercase;
      font-weight: 400;
      display: inline-block;
      // background-image: linear-gradient(
      //   to right top,
      //   #051937b7,
      //   #0a4066ab,
      //   #006b969c,
      //   #009cc398,
      //   #12ceeb81
      // );
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
  .rowl {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 6rem;
    margin-top: 5rem;
  }
  .center2 {
    display: flex;
    align-items: center;
    justify-content: center;
    border: none;

    .last1 {
      padding: 5px 14px;
      margin-bottom: -10rem;
      border-radius: 20px;
      border: none;
      transition: all 1s;
      background-image: linear-gradient(
        to right,
        #9d455b96,
        #3f5e649c,
        #41466198
      );

      .lastt {
        font-size: 1.1rem;
        color: white;

        &:hover {
          background-image: linear-gradient(
            to right,
            #9d455b96,
            #3f5e649c,
            #41466198
          );
          -webkit-background-clip: text;
          color: transparent;
          border: none;
          border-bottom: 1px solid #9d455b96;
        }
      }

      &:hover {
        background-image: linear-gradient(
          to right,
          #9d455b96,
          #3f5e649c,
          #41466198
        );
        -webkit-background-clip: text;
        color: transparent;
        border: none;
        border-radius: none;
        // border-bottom: 1px solid #9d455b96;
        // transform: translateY(-10px) translateX(10px);
        transform: scale(1.05) translateY(-0.5rem);
        box-shadow: 0 2.5rem 4rem rgba(0, 0, 0, 0.5);
        // transform: scale(0.95);
      }
    }
  }
}

.card {
  perspective: 150rem;
  -moz-perspective: 150rem;
  height: 25rem;
  width: 15rem;
  position: relative;

  .card__side {
    border-radius: 6px;
    height: 25rem;
    width: 15rem;
    transition: all 2s ease;
    position: absolute;
    overflow: hidden;
    backface-visibility: hidden;
    box-shadow: 0 1.5rem 4rem rgba(0, 0, 0, 0.4);
    &--front {
      background-color: white;
    }
    &--back {
      background-blend-mode: screen;
      transform: rotateY(180deg);
      background-size: cover;
      &-1 {
        background-image: linear-gradient(
            to bottom,
            #ffffff,
            #d4c2d7,
            #b984a0,
            #9d455b,
            #960112
          ),
          url("../assets/track1.jpg");
      }
      &-2 {
        background-image: linear-gradient(
            to bottom,
            #ffffff,
            #c1c5cc,
            #7f8f99,
            #3f5e64,
            #01302d
          ),
          url("../assets/health.jpg");
      }
      &-3 {
        background-image: linear-gradient(
            to bottom,
            #ffffff,
            #bdbcc7,
            #7e7e92,
            #414661,
            #001533
          ),
          url("../assets/nice1.jpg");
      }
    }
  }

  &:hover &__side--front {
    transform: rotateY(-180deg);
  }

  &:hover &__side--back {
    transform: rotateY(0deg);
  }

  //frontside styling
  &__picture {
    background-size: cover;
    overflow: hidden;
    height: 12rem;
    background-blend-mode: screen;
    -webkit-clip-path: polygon(0 0, 100% 0%, 100% 85%, 0% 100%);
    clip-path: polygon(0 0, 100% 0%, 100% 85%, 0% 100%);
    &--1 {
      background-image: linear-gradient(
          to bottom,
          #960112,
          #9d455b,
          #b984a0,
          #d4c2d7,
          #ffffff
        ),
        url("../assets/track2.jpg");
    }

    &--2 {
      background-image: linear-gradient(
          to bottom,
          #01302d,
          #3f5e64,
          #7f8f99,
          #c1c5cc,
          #ffffff
        ),
        url("../assets/health1.jpg");
    }

    &--3 {
      background-image: linear-gradient(
          to bottom,
          #001533,
          #414661,
          #7e7e92,
          #bdbcc7,
          #ffffff
        ),
        url("../assets/city.jpg");
    }
  }
  &__heading {
    &--1,
    &--2,
    &--3 {
      position: absolute;
      top: 7rem;
      right: 1rem;
      text-align: right;
      font-size: 1.2rem;
      font-weight: 400;
      width: 65%;
      text-transform: uppercase;
    }

    &--1 {
      background: rgb(44, 2, 2);
      -webkit-background-clip: text;
      color: transparent;
    }
    &--2 {
      background: rgb(2, 44, 30);
      -webkit-background-clip: text;
      color: transparent;
    }

    &--3 {
      background: rgb(2, 6, 44);
      -webkit-background-clip: text;
      color: transparent;
    }
  }

  &__span {
    padding: 0.2rem 0.8rem;
    -webkit-decoration-break: clone;
    &--1 {
      background-image: linear-gradient(to bottom, #9d455b94, #d4c2d7a4);
    }

    &--2 {
      background-image: linear-gradient(to bottom, #3f5e649c, #c1c5cc81);
    }

    &--3 {
      background-image: linear-gradient(to bottom, #4146619f, #bdbcc78a);
    }
  }

  &__details {
    &--1,
    &--2,
    &--3 {
      ul {
        list-style: none;
        width: 60%;
        margin: 0 auto;

        li {
          text-align: center;
          font-size: 1rem;
          font-weight: 200;
          padding: 0.4rem;
          &:not(:last-child) {
            border-bottom: 1px solid rgb(126, 126, 126);
          }
        }
      }
    }
    &--1 {
      background-image: linear-gradient(to bottom, rgb(44, 2, 2), #863c3c);
      -webkit-background-clip: text;
      color: transparent;
    }
    &--2 {
      background-image: linear-gradient(to bottom, rgb(2, 44, 31), #3c866d);
      -webkit-background-clip: text;
      color: transparent;
    }
    &--3 {
      background-image: linear-gradient(to bottom, rgb(2, 6, 44), #3c4386);
      -webkit-background-clip: text;
      color: transparent;
    }
  }
  //front side styling
  &__cta {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  &__price-box {
    text-align: center;
    margin-bottom: 10rem;
  }
  &__price-only {
    font-size: 1rem;
    text-transform: uppercase;
    &--1 {
      background: linear-gradient(
        to bottom,
        #960112,
        #9d455b,
        #b984a0,
        #d4c2d7
      );
      -webkit-background-clip: text;
      color: transparent;
    }
    &--2 {
      background-image: linear-gradient(
        to bottom,
        #01302d,
        #3f5e64,
        #7f8f99,
        #c1c5cc
      );
      -webkit-background-clip: text;
      color: transparent;
    }

    &--3 {
      background-image: linear-gradient(
        to bottom,
        #001533,
        #414661,
        #7e7e92,
        #bdbcc7
      );
      -webkit-background-clip: text;
      color: transparent;
    }
  }

  &__price-value {
    font-size: 3rem;
    font-weight: 100;
    color: rgb(87, 87, 87);
  }

  .point {
    padding: 5px 12px;
    border-radius: 10px;
    border: none;
    background: white;
    transition: all 1s;
    text-transform: uppercase;
    &__1 {
      background: linear-gradient(
        to bottom,
        #960112,
        #9d455b,
        #b984a0,
        #d4c2d7
      );
      -webkit-background-clip: text;
      color: transparent;
    }

    &__2 {
      background-image: linear-gradient(
        to bottom,
        #01302d,
        #3f5e64,
        #7f8f99,
        #c1c5cc
      );
      -webkit-background-clip: text;
      color: transparent;
    }

    &__3 {
      background-image: linear-gradient(
        to bottom,
        #001533,
        #414661,
        #7e7e92,
        #bdbcc7
      );
      -webkit-background-clip: text;
      color: transparent;
    }

    &:hover {
      transform: translateY(-10px);
    }
  }
}
</style>
