<template>
  <div class="real">
    <div class="header">
      <div class="headersub">
        <span class="headersub__first">skyspace</span>
        <span class="headersub__second">we live to save time</span>
        <button class="headersub__button">
          <span class="tag">explore</span>
        </button>
      </div>
      <div class="logo">
        <img class="logo__main" src="../assets/log.png" alt="drone log0" />
      </div>
    </div>
  </div>
  <About :Aboutpage="Aboutpage" />
  <Aboutcontent :twogrid="twogrid" />
  <Pricing :price="price" />
  <Like :liked="liked" />
  <Booking :booker="booker" />
  <Lastpage :foot="foot" />
</template>

<script>
import About from "../views/About.vue";
import Aboutcontent from "../views/Aboutcontent.vue";
import Pricing from "../views/Pricing.vue";
import Like from "../views/Like.vue";
import Booking from "../views/Booking.vue";
import Lastpage from "../views/Lastpage.vue";

export default {
  components: { About, Aboutcontent, Pricing, Like, Booking, Lastpage },
};
</script>
<style lang="scss">
* {
  margin: 0;
  padding: 0%;
}

.real {
  background: url("../assets/drone1.jpeg");
  display: relative;
  margin: 10px;
  clip-path: polygon(0 0, 100% 0%, 100% 78%, 0% 100%);
}
.header {
  font-size: 10px;
  background-image: linear-gradient(
    to right top,
    #051937,
    #0a4066ab,
    #006b969c,
    #009cc398,
    #12ceeb81
  );

  //   display: relative;
  background-size: cover;
  height: 95vh;
}
.headersub {
  position: relative;
  text-transform: uppercase;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;

  &__first {
    display: block;
    margin-bottom: 1%;
    font-weight: 400;
    font-size: 50px;
    letter-spacing: 40px;
    color: #12cfeb;
    background-image: linear-gradient(
      to bottom,
      #051937,
      #0a4066,
      #006b96,
      #009cc3dc
    );
    -webkit-background-clip: text;
    color: transparent;
    animation: first-text 5s;
  }
  &__second {
    display: block;
    margin-bottom: 60px;
    font-weight: 700;
    font-size: 20px;
    letter-spacing: 15px;
    color: rgb(32, 32, 63);
    animation: second-text 5s 2s;
  }
  &__button {
    cursor: pointer;
    display: inline-block;
    padding: 12px 50px;
    border-radius: 100px;
    background-color: rgb(230, 230, 230);
    border: none;
    text-transform: uppercase;
    animation: explore-button 5s;

    .tag {
      background-image: linear-gradient(
        to right top,
        #051937b7,
        #0a4066ab,
        #006b969c,
        #009cc398,
        #12ceeb81
      );
      -webkit-background-clip: text;
      color: transparent;
    }

    &:hover {
      transform: translateY(-3px);
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
    }
    &:active {
      transform: translateY(-1px);
      box-shadow: 10px 0 20px rgba(0, 0, 0, 0.5);
    }
  }
}
.logo {
  position: absolute;
  top: 10%;
  left: 50%;

  align-content: center;
  transform: translate(-50%, -50%);
  &__main {
    height: 12rem;
    animation: logo-drone 10s;
  }
}

@keyframes first-text {
  0% {
    opacity: 0;
    transform: translateX(-100px);
  }

  80% {
    transform: translateX(20px);
  }

  100% {
    opacity: 1;
    transform: translate(0);
  }
}

@keyframes second-text {
  0% {
    opacity: 0;
    transform: translateX(100px);
  }

  80% {
    transform: translateX(-20px);
  }

  100% {
    opacity: 1;
    transform: translate(0);
  }
}

@keyframes explore-button {
  0% {
    opacity: 0;
    transform: translateY(100px);
  }
  80% {
    transform: translateY(-20px);
  }
  100% {
    opacity: 1;
    transform: translate(0);
  }
}

@keyframes logo-drone {
  0% {
    opacity: 0;
    transform: translateX(0);
  }

  10% {
    transform: translateX(-50px);
  }
  20% {
    transform: translateX(0px);
  }

  30% {
    transform: translateX(50px);
  }

  40% {
    transform: translateX(0px);
  }
  60% {
    transform: translateY(-25px);
  }
  70% {
    transform: translateY(0px);
  }

  90% {
    transform: translateY(20px);
  }

  100% {
    opacity: 1;
    transform: translate(0);
  }
}
</style>
