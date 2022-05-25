<template>
  <section class="features">
    <div class="lines">
      <div class="col-1-in-4">
        <i class="icon-basic-world"></i>
        <h3 class="text">jncsjnsfjn</h3>
        <p>lorem ghahhjjkdk</p>
      </div>

      <div class="col-1-in-4">
        <h3 class="text">jncsjnsfjn</h3>
        <p>lorem ghahhjjkdk</p>
      </div>

      <div class="col-1-in-4">
        <h3 class="text">jncsjnsfjn</h3>
        <p>lorem ghahhjjkdk</p>
      </div>

      <div class="col-1-in-4">
        <h3 class="text">jncsjnsfjn</h3>
        <p>lorem ghahhjjkdk</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: ["twogrid"],
};
</script>

<style lang="scss">
.features {
  display: fixed;
  // clip-path: polygon(0 19%, 75% 0, 100% 0, 100% 82%, 25% 100%, 0 100%);
  // justify-content: center;
  background: linear-gradient(
    to right top,
    #051937b7,
    #0a4066ab,
    #006b969c,
    #009cc398,
    #12ceeb81
  );
  margin: 10px;
  margin-top: -10px;
  height: 95vh;
}
@mixin clearfix {
  &::after {
    content: "";
    display: table;
    clear: both;
  }
}

.lines {
  max-width: 114rem;

  position: relative;
  text-align: center;
  display: flex;
  justify-content: center;

  .col-1-in-4 {
    width: calc((100% - #{40px}) / 4);
    float: left;
    background-color: #eee;
    width: 10rem;
    height: 12rem;
    margin-top: 20%;
    margin-left: 1%;
    border-radius: 20px;
    .icon-basic-world {
      background-color: red;
      height: 20%;
      width: 20%;
    }

    .text {
      display: flex;
      justify-content: center;
      margin-top: 7rem;
      background: linear-gradient(
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

    @include clearfix;

    &:not(:last-child) {
      margin-right: 10px;
    }
  }
}
</style>
