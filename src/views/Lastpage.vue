<template>
  <footer class="footer">
    <div class="footlog">
      <img class="footl" src="../assets/log.png" alt="" />
    </div>

    <div class="footbody">
      <div class="footpa">
        <div class="footernav">
          <ul class="footerlist">
            <li class="footerit"><a href="#" class="footerlink">Company</a></li>
            <li class="footerit"><a href="#" class="footerlink">Contact</a></li>
            <li class="footerit"><a href="#" class="footerlink">sector</a></li>
            <li class="footerit"><a href="#" class="footerlink">about</a></li>
            <li class="footerit"><a href="#" class="footerlink">Company</a></li>
          </ul>
        </div>
      </div>

      <div class="footpa">
        <div class="footpap">
          <p class="footerpra">
            Lorem Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut
            pariatur nobis error quas esse iste ipsa expedita ad libero?
            Voluptatum corrupti aspernatur reprehenderit maxime dicta vitae
            deserunt, optio Lorem ipsum dolor sit amet consectetur adipisicing
            elit. Ut pariatur nobis error quas esse iste ipsa expedita ad
            libero? Voluptatum corrupti aspernatur
          </p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  prop: ["foot"],
};
</script>

<style lang="scss">
.footer {
  padding: 8rem 0;
  background: rgb(41, 41, 41);
  font-size: 1rem;
  .footlog {
    text-align: center;
    margin-top: -12rem;
  }
  .footl {
    width: 15rem;
    height: auto;
  }
}
.footbody {
  height: 100%;
  width: 100%;
  display: inline-flex;
  gap: 5rem;

  .footpa {
    display: inline-block;
    height: 60%;
    width: 60%;
  }
}
.footerlist {
  font-size: 0.9rem;
  margin-left: 2rem;
  text-align: center;
  list-style: none;
}
.footerit {
  display: inline-block;
  &:not(:last-child) {
    margin-right: 2rem;
  }
}
.footernav {
  border-top: #009cc398 solid 2px;
  padding-top: 1rem;
  display: inline-block;
  margin-left: 12rem;
}

.footerlink {
  &:visited,
  &:link {
    background-image: linear-gradient(to right, #9d455bea, #3f5e64e1);
    border: none;
    -webkit-background-clip: text;
    color: transparent;
    display: inline-block;
    text-decoration: none;
    text-transform: uppercase;
    transition: all 0.8s;
  }
  &:hover,
  &:active {
    color: #009cc3de;
    box-shadow: 0 1rem 2rem rgba(#000000, 0.4);
    transform: rotate(5deg) scale(1.3);
  }
}

.footpap {
  border-top: #009cc398 solid 2px;
  display: inline-block;
  margin-right: 12rem;
  padding-top: 1rem;
}
.footerpra {
  background-image: linear-gradient(to right top, #006b96, #009cc3, #12ceeb);
  -webkit-background-clip: text;
  color: transparent;
}
</style>
