<template>
  <div id="content">
    <img
      class="img-top fixed"
      v-bind:class="{
        'star-sky': isClickedMore,
        about_clicked_sky: afterIsClickedAbout
      }"
      src="@/assets/img/background.png"
    />
    <img
      class="the_way fixed"
      v-bind:class="{ way_skew: isClickedMore }"
      src="@/assets/img/the_way.png"
    />

    <div
      class="sun fixed "
      v-bind:class="{
        out_of_page1: isClickedMore,
        click_about_sun: isClickedAbout
      }"
    ></div>
    <img
      class="the_cloud fixed "
      v-bind:class="{ fadeOut: afterIsClickedAbout }"
      src="@/assets/img/the_clouds.png"
    />
    <img
      class="animated-image the_mosque fixed "
      v-bind:class="{
        'mosque-bottom': isClickedMoreThen,
        'mosque-to-bottom': isClickedMore,
        click_about_mosque: isClickedAbout
      }"
      src="@/assets/img/the mosque.png"
    />
    <img
      class="the_towers fixed "
      v-bind:class="{
        the_towers_to_bottom: isClickedMore,
        'tower-bottom': isClickedMoreThen,
        click_about_mosque: isClickedAbout
      }"
      src="@/assets/img/the_towers.png"
    />

    <img
      class="animated-image the_little_towers fixed "
      v-bind:class="{
        the_little_to_bottom: isClickedMore,
        the_little: isClickedMoreThen,
        about_clicked_after: afterIsClickedAbout
      }"
      src="@/assets/img/the_little_towers.png"
    />
    <div id="social" class="fixed" v-bind:class="{ fadeOut: isClickedMore }">
      <a href="#">
        <i class="fa fa-phone fa-flip-horizontal"></i>
      </a>
      <a href="#">
        <i class="far fa-envelope"></i>
      </a>
      <a href="#">
        <i class="far fa-question-circle "></i>
      </a>
    </div>
    <button
      class="fixed about"
      v-on:click="aboutUsClicked"
      v-bind:class="{ fadeOut: isClickedMore }"
    >
      About us <span></span>
    </button>

    <button class="fixed btn lets_go" v-bind:class="{ fadeOut: isClickedMore }">
      Let's go
    </button>

    <button
      class="fixed download-app "
      v-bind:class="{ fadeOut: isClickedMore || isClickedAbout }"
      href="#"
    >
      Download app <i class="fa fa-download"></i>
    </button>
    <button
      class="more-info fixed btn"
      v-on:click="more"
      v-bind:class="{ fadeOut: isClickedMore || isClickedAbout }"
    >
      Batafsil
    </button>

    <div class="fixed message" :class="isActiveMessage ? 'fadeIn' : 'fadeOut'">
      <a v-on:click="toHome" class="back"><i class="fas fa-arrow-left"></i></a>
      <div class="content">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, quae
        architecto nulla veritatis sequi fugiat nemo nihil facilis facere
        blanditiis exercitationem maxime dolores voluptatum placeat harum libero
        eveniet. Suscipit, sed.
      </div>
    </div>

    <div
      class="fixed about-container"
      v-on:click="aboutUsClicked"
      :class="afterIsClickedAbout ? 'fadeIn' : 'fadeOut'"
    >
      <div class="about-content">
        <span>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Adipisci
          numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem ipsum dolor sit amet
          consectetur adipisicing elit. Adipisci numquam quas laboriosam enim!
          Totam corrupti earum quam nisi, praesentium voluptas ratione, autem
          veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Adipisci numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem iLorem ipsum dolor sit
          amet consectetur adipisicing elit. Adipisci numquam quas laboriosam
          enim! Totam corrupti earum quam nisi, praesentium voluptas ratione,
          autem veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Adipisci numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem ipsum dolor sit amet
          consectetur adipisicing elit. Adipisci numquam quas laboriosam enim!
          Totam corrupti earum quam nisi, praesentium voluptas ratione, autem
          veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem iLorem ipsum dolor sit amet consectetur adipisicing
          elit. Adipisci numquam quas laboriosam enim! Totam corrupti earum quam
          nisi, praesentium voluptas ratione, autem veritatis quis dolorem
          molestias quod, consequuntur consequatur cumque. Lorem ipsum dolor sit
          amet consectetur adipisicing elit. Adipisci numquam quas laboriosam
          enim! Totam corrupti earum quam nisi, praesentium voluptas ratione,
          autem veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Adipisci numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem iLorem ipsum dolor sit
          amet consectetur adipisicing elit. Adipisci numquam quas laboriosam
          enim! Totam corrupti earum quam nisi, praesentium voluptas ratione,
          autem veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Adipisci numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem ipsum dolor sit amet
          consectetur adipisicing elit. Adipisci numquam quas laboriosam enim!
          Totam corrupti earum quam nisi, praesentium voluptas ratione, autem
          veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem iLorem ipsum dolor sit amet consectetur adipisicing
          elit. Adipisci numquam quas laboriosam enim! Totam corrupti earum quam
          nisi, praesentium voluptas ratione, autem veritatis quis dolorem
          molestias quod, consequuntur consequatur cumque. Lorem ipsum dolor sit
          amet consectetur adipisicing elit. Adipisci numquam quas laboriosam
          enim! Totam corrupti earum quam nisi, praesentium voluptas ratione,
          autem veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Adipisci numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem ipsum dolor sit amet
          consectetur adipisicing elit. Adipisci numquam quas laboriosam enim!
          Totam corrupti earum quam nisi, praesentium voluptas ratione, autem
          veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Adipisci numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem ipsum dolor sit amet
          consectetur adipisicing elit. Adipisci numquam quas laboriosam enim!
          Totam corrupti earum quam nisi, praesentium voluptas ratione, autem
          veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Adipisci numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem iLorem ipsum dolor sit
          amet consectetur adipisicing elit. Adipisci numquam quas laboriosam
          enim! Totam corrupti earum quam nisi, praesentium voluptas ratione,
          autem veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Adipisci numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem ipsum dolor sit amet
          consectetur adipisicing elit. Adipisci numquam quas laboriosam enim!
          Totam corrupti earum quam nisi, praesentium voluptas ratione, autem
          veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem iLorem ipsum dolor sit amet consectetur adipisicing
          elit. Adipisci numquam quas laboriosam enim! Totam corrupti earum quam
          nisi, praesentium voluptas ratione, autem veritatis quis dolorem
          molestias quod, consequuntur consequatur cumque. Lorem ipsum dolor sit
          amet consectetur adipisicing elit. Adipisci numquam quas laboriosam
          enim! Totam corrupti earum quam nisi, praesentium voluptas ratione,
          autem veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Adipisci numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem iLorem ipsum dolor sit
          amet consectetur adipisicing elit. Adipisci numquam quas laboriosam
          enim! Totam corrupti earum quam nisi, praesentium voluptas ratione,
          autem veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Adipisci numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem ipsum dolor sit amet
          consectetur adipisicing elit. Adipisci numquam quas laboriosam enim!
          Totam corrupti earum quam nisi, praesentium voluptas ratione, autem
          veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem iLorem ipsum dolor sit amet consectetur adipisicing
          elit. Adipisci numquam quas laboriosam enim! Totam corrupti earum quam
          nisi, praesentium voluptas ratione, autem veritatis quis dolorem
          molestias quod, consequuntur consequatur cumque. Lorem ipsum dolor sit
          amet consectetur adipisicing elit. Adipisci numquam quas laboriosam
          enim! Totam corrupti earum quam nisi, praesentium voluptas ratione,
          autem veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque. Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Adipisci numquam quas laboriosam enim! Totam corrupti earum quam nisi,
          praesentium voluptas ratione, autem veritatis quis dolorem molestias
          quod, consequuntur consequatur cumque. Lorem ipsum dolor sit amet
          consectetur adipisicing elit. Adipisci numquam quas laboriosam enim!
          Totam corrupti earum quam nisi, praesentium voluptas ratione, autem
          veritatis quis dolorem molestias quod, consequuntur consequatur
          cumque.
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {},
  data() {
    return {
      isClickedMore: false,
      isClickedMoreThen: false,
      isActiveMessage: false,

      isClickedAbout: false,
      afterIsClickedAbout: false
    };
  },
  methods: {
    more() {
      this.isClickedMore = !this.isClickedMore;
      setTimeout(() => {
        this.isClickedMoreThen = !this.isClickedMoreThen;
      }, 3000);
      setTimeout(() => {
        this.isActiveMessage = !this.isActiveMessage;
      }, 5000);
    },
    toHome() {
      this.isClickedMore = !this.isClickedMore;
      this.isClickedMoreThen = !this.isClickedMoreThen;
      this.isActiveMessage = !this.isActiveMessage;
    },
    aboutUsClicked() {
      this.isClickedAbout = !this.isClickedAbout;
      setTimeout(() => {
        this.afterIsClickedAbout = !this.afterIsClickedAbout;
      }, 2000);
    }
  }
};
</script>

<style lang="scss" scoped>
.message {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  opacity: 0;
  top: 10vh;
  left: 10vw;
  width: 80vw;
  height: 80vh;
  padding: 10px;
  // background-color: white;
  .back {
    color: white;
    padding: 8px 10px;
    display: flex;
    align-items: center;
    justify-content: flex-start;
    max-width: 50px;
    border-radius: 5px;
    &:hover {
      cursor: pointer;
      color: rgb(153, 149, 149);
    }
    // background-color: rgb(201, 184, 34);
  }
  .content {
    padding: 10px;
    width: 100%;
    height: 100%;
    background-color: lemonchiffon;
  }
}

.mosque-to-bottom {
  transition: all 2s ease-in-out;

  transform: translate(0, 240px) scale(0.5);
}
.the_little_to_bottom {
  transition: all 1s ease-in-out;
  transform: translate(0, 260px) scale(0.5) skewY(-6deg);
}
.the_towers_to_bottom {
  transition: all 2s ease-in-out;
  transform: translate(0, 312px) scale(0.5);
}
.mosque-bottom {
  transition: all 2s ease-in-out;

  transform: translate(-200px, 240px) scale(0.5);
}
.the_little {
  transition: all 1s ease-in-out;

  transform: translate(-200px, 250px) scale(0.6, 0.6) skewY(-6deg);
}
.tower-bottom {
  transition: all 2s ease-in-out;
  transform: translate(-200px, 312px) scale(0.5);
}
.star-sky {
  transition: all 2.3s ease-in-out;
  transform: skewY(-4.5deg) scaleY(1.6) translateY(50px);
}
.way_skew {
  transition: all 3.5s ease-in-out;
  transform: skewY(-4deg) translateY(150px);
}

.out_of_page1 {
  // outline: 1px solid red;
  transition: all 10s ease-in-out;
  transform: translate(500px, -500px);
  opacity: 0;
}
.fadeOut {
  transition: all 1s ease-in-out;
  opacity: 0;
  visibility: hidden;
}
#content {
  width: 100%;
  height: 100vh;
  $diameter-sun: 430px;
  position: relative;
  .about-container {
    width: 100%;

    .about-content {
      display: flex;
      width: 40vw;
      height: 70vh;
      margin-top: 50px;
      margin-left: 30px;
      border-radius: 40px;

      padding: 30px 10px;
      // padding: 10px;
      background-color: white;
      span {
        &::-webkit-scrollbar {
          width: 5px;
          // background-color: rgb(162, 5, 162);
        }

        &::-webkit-scrollbar-track {
          width: 2.5px;
          border-radius: 20px;
          background-color: rgb(162, 5, 162);
        }
        &::-webkit-scrollbar-thumb {
          outline: 4px solid rgb(162, 5, 162);
          background-color: rgb(162, 5, 162);
          border-radius: 20px;
          max-height: 20px;
          &:hover {
            transition: all 0.3s ease-in-out;
            background-color: rgb(92, 15, 92);
            outline: 4px solid rgb(92, 15, 92);
          }
        }
        width: 100%;
        height: 100%;
        padding-right: 10px;
        overflow-y: scroll;
        text-overflow: ellipsis;
      }
    }
    z-index: 5;
    height: 100vh;
  }
  .about {
    position: relative;
    background: none;
    z-index: 4;
    border: none;
    outline: none;
    top: 30px;
    color: white;
    font-weight: 700;
    font-size: 23px;
    right: 300px;
    animation: fadeIn 3s ease-in-out;
    overflow: hidden;
    padding: 4px;

    &:hover {
      cursor: pointer;
    }
    &:hover span {
      transition: all 0.2s ease-in-out;
      transform: translateX(100%);
    }
    span {
      transition: all 0.5s ease-in-out;
      position: absolute;
      left: -100%;

      width: 100%;
      height: 2px;
      background-color: lemonchiffon;
    }
  }
  .lets_go {
    z-index: 4;
    top: 20px;
    right: 30px;
    padding: 10px 20px;
    color: rgb(110, 30, 167);
    font-weight: 900;
    transition: all 0.2s ease-in-out;
    background-color: white;
    animation: fadeIn 3s ease-in-out;
    &:hover {
      transition: all 0.2s ease-in-out;
      right: 25px;
      padding: 12px 25px;
    }
  }
  .fixed {
    position: fixed;
  }
  .btn {
    z-index: 4;
    transition: all 3s ease-in-out;
    font-size: 16px;
    letter-spacing: 1px;
    border-radius: 25px;
    outline: none;
    border: 2px solid white;
    &:hover {
      cursor: pointer;
    }
  }
  .more-info {
    color: white;
    bottom: 100px;
    padding: 10px 50px;
    background-color: inherit;
    left: 242px;
    padding: 10px 50px;
    transition: all 0.5s ease;
    &:hover {
      background-color: white;
      transition: all 0.5s ease;
      color: inherit;
    }
  }
  .download-app {
    bottom: 15px;
    left: 90px;
    background: none;
    outline: none;
    border: none;
    transition: all 1s ease-in-out;
    color: white;
    font-size: 25px;
    animation: fadeIn 5s ease-in-out;
  }
  .the_cloud {
    width: 100%;
    height: 100vh;
    transition: all 2s ease-in-out;
    animation: inBottom-cloud 2s ease-in-out;
  }
  .sun {
    opacity: 1;
    width: $diameter-sun;
    top: 70px;
    right: 225px;
    height: $diameter-sun;
    box-shadow: 6px 6px 20px white, -6px -6px 20px white;
    background-color: white;
    transition: all 4s ease-in-out;
    animation: inBottom 2.8s ease-in-out;
    border-radius: 50%;
  }
  $width-imgs: 92%;
  $height-imgs: 95vh;
  .animated-image {
    width: $width-imgs;
    height: $height-imgs;
    bottom: 0;
    right: -60px;
  }
  .the_little_towers {
    z-index: 3;
    transition: all 3.5s ease-in-out;
    animation: inTop 4.6s ease-in-out;
  }
  .the_towers {
    transition: all 3s ease-in-out;

    width: $width-imgs;
    height: $height-imgs;
    right: -60px;
    z-index: 3;
    bottom: 0;
    animation: inTop 3.3s ease-in-out;
  }
  .img-top {
    transition: all 3s ease-in-out;
    width: 100%;
    height: 100%;
    top: 0;
  }
  .the_mosque {
    transition: all 3s ease-in-out;
    right: -60px;
    bottom: 0;
    z-index: 3;
    animation: inTop 3s ease-in-out;
  }

  .the_way {
    transition: all 3s ease-in-out;

    width: 100%;
    height: 100%;
  }
  #social {
    transition: all 1s ease-in-out;

    display: flex;
    flex-direction: column;
    min-width: 20px;
    bottom: 15px;
    left: 3px;
    animation: fadeIn 5s ease-in-out;
    a {
      color: white;
      font-size: 28px;
    }
  }
}

.click_about_mosque,
.about_clicked_after {
  filter: blur(1px);
  transform: translate(100px, 60px) scale(0.96);
}
.click_about_sun {
  transform: translate(100px, 60px);
}
.about_clicked_after {
  transform: scaleX(0.9) translate(130px, 60px);
}
.about_clicked_sky {
  transform: scale(1.1) translate(10px, 10px);
  filter: blur(1px);
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@keyframes inTop {
  from {
    transform: translate(0, 500px);
  }
  to {
    transform: translate(0, 0);
  }
}
@keyframes inBottom-cloud {
  from {
    transform: translate(0, -200px);
    opacity: 0;
  }
  to {
    opacity: 1;
    transform: translate(0, 0);
  }
}
@keyframes inBottom {
  from {
    transform: translate(0, -500px);
  }
  to {
    transform: translate(0, 0);
  }
}
.fadeIn {
  display: flex;
  visibility: visible;
  transition: opacity 0.3s ease-in;
  opacity: 1;
}
</style>
