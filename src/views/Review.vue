<template>
  <section class="reviewbody">
    <div class="bgvid">
      <video class="bgvideo">
        <source src="../assets/life.mp4" />
      </video>
    </div>

    <div class="headerrev">
      <h3 class="textrev">what you think about us</h3>
    </div>
    <div class="all">
      <div class="bodyrev">
        <div class="circlerev">mmmmm</div>
        <div class="picrev"></div>
        <h3 class="textheadrev">thank you jesus</h3>
        <p class="parafrev">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut pariatur
          nobis error quas esse iste ipsa expedita ad libero? Voluptatum
          corrupti aspernatur reprehenderit maxime dicta vitae deserunt, optio
        </p>
      </div>

      <div class="bodyrev">
        <div class="circlerev">mmmmm</div>
        <div class="picrev"></div>
        <h3 class="textheadrev">thank you jesus</h3>
        <p class="parafrev">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut pariatur
          nobis error quas esse iste ipsa expedita ad libero? Voluptatum
          corrupti aspernatur reprehenderit maxime dicta vitae deserunt, optio
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: ["rev"],
};
</script>

<style lang="scss">
.reviewbody {
  padding: 11rem 0;
  margin: -10px 10px;
  background-image: linear-gradient(
    to right top,
    #051937b7,
    #0a4066ab,
    #006b969c,
    #009cc398,
    #12ceeb81
  );
  text-align: center;

  .headerrev {
    text-transform: uppercase;
    font-size: 2rem;

    .textrev {
      font-weight: 400;
      padding: 5px 12px;
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
      margin-top: -10rem;
      margin-bottom: 5rem;
      text-align: center;
    }
  }
  .all {
    display: flex;
    flex-direction: column;
    gap: 30px;
    .bodyrev {
      padding: 1rem;
      margin-bottom: 2rem;
      background-color: rgba(238, 238, 238, 0.8);
      width: 75%;
      height: 10rem;
      margin: 0 auto;
      clip-path: polygon(0% 0%, 95% 0%, 100% 100%, 5% 100%);
      .circlerev {
        background-color: cyan;
        // padding: 10px 10px;
        margin-top: 2rem;
        margin-left: 3rem;
        width: 100px;
        height: 100px;
        clip-path: circle(50% at 50% 50%);
      }
      .textheadrev {
        text-transform: uppercase;
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
        margin-top: -5rem;
        display: block;
        margin-bottom: 1rem;
        margin-left: 18%;
        text-align: left;
      }

      .parafrev {
        text-align: left;
        margin-left: 18%;
        color: black;
      }
    }
  }
}
</style>
