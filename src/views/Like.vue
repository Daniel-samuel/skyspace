<template>
  <section class="likeme">
    <div class="bgvid">
      <video class="bgvideo" autoplay muted loop>
        <source src="../assets/life.mp4" />
      </video>
    </div>

    <div class="likehead">
      <h3 class="liketext">why you like us</h3>
    </div>
    <div class="allcont">
      <div class="likecontainer">
        <figure class="likecircle">
          <img src="../assets/pop2.jpg" alt="image" class="likeimg" />
          <figcaption class="likecap">kingsley sunday</figcaption>
        </figure>

        <div class="likebody">
          <h3 class="likebodytext">i had the best week with my family</h3>
          <p class="likepara">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut pariatur
            nobis error quas esse iste ipsa expedita ad libero? Voluptatum
            corrupti aspernatur reprehenderit maxime dicta vitae deserunt, optio
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut pariatur
            nobis error quas esse iste ipsa expedita ad libero? Voluptatum
            corrupti aspernatur
          </p>
        </div>
      </div>

      <div class="likecontainer">
        <figure class="likecircle">
          <img src="../assets/pop3.jpg" alt="image" class="likeimg" />
        </figure>

        <div class="likebody">
          <h3 class="likebodytext">i had the best week with my family</h3>
          <p class="likepara">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut pariatur
            nobis error quas esse iste ipsa expedita ad libero? Voluptatum
            corrupti aspernatur reprehenderit maxime dicta vitae deserunt, optio
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut pariatur
            nobis error quas esse iste ipsa expedita ad libero? Voluptatum
            corrupti aspernatur
          </p>
        </div>
      </div>
    </div>

    <div class="likebutton">
      <button class="likethe">
        <span class="bottext">More Reviews</span>
      </button>
    </div>
  </section>
</template>

<script>
export default {
  props: ["liked"],
};
</script>

<style lang="scss">
.likeme {
  height: 100%;
  position: relative;
  padding: 1rem;
  margin: -10px 10px;
  background-image: linear-gradient(
    to right top,
    #051937b7,
    #0a4066ab,
    #006b969c,
    #009cc398,
    #12ceeb81
  );

  .likehead {
    .liketext {
      text-transform: uppercase;
      font-size: 35px;
      font-weight: 400;
      padding: 5px 12px;
      margin-top: 2rem;
      text-align: center;
      margin-bottom: 2rem;
      background-image: linear-gradient(
        to right top,
        #051937,
        #0a4066,
        #006b96
      );
      -webkit-background-clip: text;
      color: transparent;
    }
  }
  .allcont {
    display: flex;
    flex-direction: column;
    gap: 1rem;

    .likecontainer {
      padding: 2rem;
      //   margin-bottom: 1rem;
      background-color: rgba(238, 238, 238, 0.8);
      width: 70%;
      margin: 0 auto;
      clip-path: polygon(5% 0, 100% 0%, 95% 100%, 0% 100%);
      transition: all 3s;

      .likecircle {
        float: left;
        shape-outside: circle(50% at 50% 50%);
        clip-path: circle(43% at 50% 50%);
        transform: translateX(-1rem);
        background-size: cover;
        position: relative;
        transition: all 3s;
        &:hover &.likecap {
          opacity: 1;
          transform: translateY(-50%);
        }
      }
      .likeimg {
        width: 7rem;
        //   transition: all 0.5s;
      }
      .likecap {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-10%, -20%);
        text-align: center;
        text-transform: uppercase;
        color: white;
        opacity: 0;
        transition: all 0.5s;

        &:hover {
          opacity: 1;
          transform: translateX(-50%);
        }
      }

      .likebody {
        padding: 1rem;
        .likebodytext {
          color: #009cc398;
          text-transform: uppercase;
          margin-top: -1rem;
          margin-bottom: 1rem;
        }
      }
      //   &:hover &.likecap {
      //     opacity: 1;
      //     transform: translateY(-40%);
      //   }
    }
  }
  .likebutton {
    text-align: center;
    margin-top: 4rem;
    .likethe {
      padding: 7px 14px;
      border: none;
      background-image: linear-gradient(to right, #eee);
      -webkit-background-clip: text;
      color: transparent;
      transition: all 1s;

      .bottext {
        font-size: 18px;
        border-bottom: 1px solid #009cc398;
      }

      &:hover {
        // color: white;
        border-radius: 20px;

        background-image: linear-gradient(to right top, #006b969c, #009cc398);
        -webkit-background-clip: text;
        color: transparent;
        transform: scale(1.05) translateY(-0.5rem);
        box-shadow: 0 2.5rem 4rem rgba(0, 0, 0, 0.5);
      }
    }
  }
}
.bgvid {
  height: 100%;
  width: 100%;
  position: absolute;
  object-fit: cover;
  top: 0;
  left: 0;
  z-index: -1;

  .bgvideo {
    height: 100%;
    width: 100%;
    object-fit: cover;
    -o-object-fit: cover;
  }
}
</style>
