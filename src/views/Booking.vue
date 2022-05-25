<template>
  <section class="book">
    <div class="book_box">
      <div class="pixx">
        <div class="dform">
          <form action="#" class="form">
            <div class="bookhead">
              <h3 class="booktext">start booking now</h3>
            </div>
            <div class="form__group">
              <input
                type="text"
                class="form__name"
                placeholder="Full Name"
                id="name"
                required
              />
              <label for="name" class="form__label">Full Name</label>
            </div>

            <div class="form__group">
              <input
                type="email"
                class="form__name"
                placeholder="Email address"
                id="mail"
                required
              />
              <label for="mail" class="form__label">Email Address</label>
            </div>

            <div class="form__group">
              <input
                type="text"
                class="form__name"
                placeholder="Location"
                id="locate"
                required
              />
              <label for="locate" class="form__label">Location</label>
            </div>

            <div class="form__group">
              <div class="form__radio--group">
                <input
                  type="radio"
                  class="form__radio--input"
                  id="small"
                  name="size"
                />
                <label for="small" class="form__radio-label">
                  <span class="form__radio--button">
                    <span class="butt">Tracking</span>
                  </span>
                </label>
              </div>

              <div class="form__radio--group">
                <input
                  type="radio"
                  class="form__radio--input"
                  id="large"
                  name="size"
                />
                <label for="large" class="form__radio-label">
                  <span class="form__radio--button">
                    <span class="butt">Medical</span>
                  </span>
                </label>
              </div>

              <div class="form__radio--group">
                <input
                  type="radio"
                  class="form__radio--input"
                  id="xlarge"
                  name="size"
                />
                <label for="xlarge" class="form__radio-label">
                  <span class="form__radio--button">
                    <span class="butt">Delivery</span>
                  </span>
                </label>
              </div>
            </div>
            <div class="submit">
              <button class="submitbutton">Next Step &rarr;</button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  prop: ["booker"],
};
</script>

<style lang="scss">
.book {
  height: 85vh;
  margin: 10px 10px;
  background: #eee;

  justify-content: center;
  align-items: center;
}

.book_box {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 20rem;
  margin: 0 auto;
  display: flex;

  height: 100%;
  width: 100%;
}

.pixx {
  height: 70%;
  width: 80%;
  background-image: linear-gradient(
      105deg,
      rgba(#9d455b94, 0.5) 0%,
      rgba(#3f5e649c, 0.6) 25%,
      rgba(#4146619f, 0.6) 50%,
      transparent 50%
    ),
    url(../assets/done2.jpeg);
  border-radius: 6px;
  // padding: 13rem 35rem;
  background-size: cover;
}

.dform {
  width: 50%;
  height: 100%;
}

.form {
  &__group {
    margin-bottom: 1rem;
    margin-left: 2rem;
  }
  &__name {
    padding: 5px 2rem;
    color: rgb(51, 51, 51);
    border-radius: 2px;
    background-color: rgba(238, 238, 238, 0.671);
    border: none;
    font-size: 1rem;
    border-bottom: transparent solid 3px;
    width: 70%;
    display: block;
    transition: all 0.3s;

    &:focus {
      outline: none;
      box-shadow: rgba(0, 0, 0, 0.1);
      border-bottom: #3f5e64 solid 3px;
      border-radius: none;
    }

    &:focus:invalid {
      border-bottom: brown solid 3px;
    }

    &::-webkit-input-placeholder {
      color: #999;
    }
  }
  &__label {
    font-size: 0.8rem;
    font-weight: 500;
    margin-left: 2rem;
    margin-top: 0.5rem;
    display: block;
    transition: all 0.4s;
  }

  &__name:placeholder-shown + &__label {
    opacity: 0;
    visibility: hidden;
    transform: translateY(-3rem);
  }

  &__radio--group {
    width: 30%;
    display: inline-block;
  }
  &__radio--input {
    display: none;
  }

  &__radio-label {
    font-size: 1rem;
    font-weight: 500;

    position: relative;
  }

  &__radio--button {
    position: relative;
    height: 1rem;
    width: 1rem;
    border: 2px solid red;
    border-radius: 50%;
    display: inline-block;
    left: 0rem;
    top: 0rem;
    &::after {
      content: "";
      display: block;
      height: 0.7rem;
      width: 0.7rem;
      border-radius: 50%;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background-color: red;
      opacity: 0;
      transition: opacity 1;
    }
    .butt {
      left: 2rem;
      top: -0.05rem;
      cursor: pointer;
      position: absolute;
      transition: all 0.4s;
    }
    &__radio--input:checked + &__radio-label + &__radio--button::after .butt {
      opacity: 1;
    }
  }

  .submit {
    padding: 6px 10px;

    position: relative;
    .submitbutton {
      cursor: pointer;
      position: absolute;
      padding: 10px 2.5rem;
      left: 0rem;
      border-radius: 10px;
      border: none;
      background-image: linear-gradient(
        to right top,
        #051937,
        #0a4066,
        #006b96
      );
      -webkit-background-clip: text;
      color: transparent;
      font-weight: 500;
      font-size: 1rem;

      transition: all 0.6;
      &:hover {
        color: black;
        background-image: linear-gradient(to right, #414661, #414661, #9d455b);
        -webkit-background-clip: text;
        color: transparent;
        transform: scale(1.05) translateY(-0.5rem);
      }
    }
  }
}

.bookhead {
  display: flex;
  justify-content: left;
}
.booktext {
  font-size: 30px;
  font-weight: 500;
  text-transform: uppercase;
  margin-top: 50px;
  margin-bottom: 50px;
  margin-left: 2rem;
}
</style>
