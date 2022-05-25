<template>
  <div class="over">
    <section class="features">
      <div class="rows">
        <div class="col-1-of-4">
          <div class="feature-box">
            <img src="../assets/_SVG/basic_world.svg" alt="" class="imgg" />
            <h3 class="newhead">all over the world</h3>
            <p class="newheadp">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut
              pariatur
            </p>
          </div>
        </div>

        <div class="col-1-of-4">
          <div class="feature-box">
            <img src="../assets/_SVG/basic_clockwise.svg" alt="" class="imgg" />
            <h3 class="newhead">always on time</h3>
            <p class="newheadp">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut
              pariatur
            </p>
          </div>
        </div>

        <div class="col-1-of-4">
          <div class="feature-box">
            <img src="../assets/_SVG/basic_map.svg" alt="" class="imgg" />
            <h3 class="newhead">find your way</h3>
            <p class="newheadp">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut
              pariatur
            </p>
          </div>
        </div>

        <div class="col-1-of-4">
          <div class="feature-box">
            <img
              src="../assets/_SVG/basic_geolocalize-05.svg"
              alt=""
              class="imgg"
            />
            <h3 class="newhead">door step delivery</h3>
            <p class="newheadp">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut
              pariatur
            </p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  props: ["twogrid"],
};
</script>

<style lang="scss">
.over {
  // width: 100%;
  transform: skewY(-7deg);
  background: url("../assets/drone1.jpeg");
  // background-size: cover;
  margin: 10px;
  height: 90vh;
  margin-top: -10rem;
}
.features {
  height: 90vh;
  width: auto;
  background-image: linear-gradient(
    to right top,
    #051937b7,
    #0a4066ab,
    #006b969c,
    #009cc398,
    #12ceeb81
  );
}

.rows {
  transform: skewY(7deg);
  display: flex;
  flex-wrap: wrap;
  gap: 50px;
  flex-shrink: 0;
  justify-content: center;
  justify-items: center;
  align-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  .col-1-of-4 {
    width: 200px;
    height: auto;
  }
}

.feature-box {
  background-color: rgba(238, 238, 238, 0.8);
  font-size: 1.6;
  padding: 1.5rem;
  text-align: center;
  border-radius: 3px;
  box-shadow: 0 1.5rem 4rem rgba(0, 0, 0, 0.15);
  transition: transform 0.3s;

  .imgg {
    font-size: 6rem;
    margin-bottom: 0.5rem;
  }
  &:hover {
    transform: translateY(-2rem) scale(1.03);
    box-shadow: 0 1.5rem 4rem rgba(0, 0, 0, 0.637);
  }

  .newhead {
    text-transform: uppercase;
    font-size: 13px;
  }
  .newheadp {
    font-size: 14px;
  }
}

// $bg-img: url("../assets/time.jpg");
</style>
