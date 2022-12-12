<template>
  <div class="home">
    <div class="hero">
      <div class="container">
        <div class="hero_text">
          <h2 class="hero_text_title">MEAL Center for your brands.</h2>
          <p class="hero_text_desc">
            Otto is the best software platform to easily capture user feed back
            for your brand and products.
          </p>
          <a class="hero_text_bottom" href="#">meal center yemen</a>
        </div>

        <div class="hero_photo">
          <div class="container position-relative">
            <img
              class="hero_photo_Component"
              src="../assets/hero_Component.svg"
              alt="hero_Component"
            />
            <img
              class="hero_photo_dashboard"
              src="../assets/hero_dashboard.svg"
              alt="hero_dashboard"
            />
            <img
              class="hero_photo_Component1"
              src="../assets/hero_Component1.svg"
              alt="hero_Component1"
            />
          </div>
        </div>
      </div>
    </div>

    <!-- start services -->
    <div class="services">
      <div class="container">
        <h3>Our Services</h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing ,ipsum dolor sit
          amet, consectetur adipiscing.
          Lorem ipsum dolor sit amet, consectetur adipiscing ,ipsum dolor sit
          amet, consectetur adipiscing.
        </p>
        <div class="row">
          <div class="col-lg-3">
            <div class="services_container">
              <div class="services_container_img">
                <img src="../assets/aboutIcon 1.svg" alt="aboutIcon 3.svg" />
              </div>
              <div class="services_container_text">
                <h4>
                  Web <br />
                  Desging
                </h4>
              </div>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="services_container">
              <div class="services_container_img">
                <img src="../assets/aboutIcon 2.svg" alt="aboutIcon 3.svg" />
              </div>
              <div class="services_container_text">
                <h4>
                  App <br />
                  Desging
                </h4>
              </div>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="services_container">
              <div class="services_container_img">
                <img src="../assets/aboutIcon 3.svg" alt="aboutIcon 3.svg" />
              </div>
              <div class="services_container_text">
                <h4>
                  App <br />
                  Desging
                </h4>
              </div>
            </div>
          </div>
          <div class="col-lg-3">
            <div class="services_container">
              <div class="services_container_img">
                <img src="../assets/aboutIcon 1.svg" alt="aboutIcon 3.svg" />
              </div>
              <div class="services_container_text">
                <h4>
                  Web <br />
                  Desging
                </h4>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- end services -->

    <!-- start about_us -->
    <div class="aboutus">
      <div class="container">
        <div class="row">
          <div class="col-lg-6">
            <div class="aboutus_imgside">
              <img src="../assets/about_ Image.svg" alt="about_ Image" />
            </div>
          </div>
          <div class="col-lg-6">
            <div class="aboutus_textside">
              <h4 class="aboutus_textside_heading">about us</h4>
              <p class="aboutus_textside_desc">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. In
                pretium, elit quis vehicula interdum, sem metus iaculis sapien,
                sed bibendum lectus augue eu metus.
              </p>
              <div></div>
              <a class="aboutus_textside_link" href="#">
                <span>read more</span>
                <img src="../assets/link_arow.svg" alt="link_arow" />
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- end about_us -->

    <!-- start feedback -->
    <div class="feedback">
      <div class="container">
        <h3>Testimonials from clients</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing.</p>
        <feed-back
          v-for="feedbacks in slides"
          :key="feedbacks.id"
          :feedbacks="feedbacks"
        />
      </div>
    </div>
    <!-- End feedback -->

    <!-- start supporter -->
    <div class="suppoter">
      <div class="container">
        <h2>Meal Center team is trusted by</h2>
        <div class="suppoter_container">
          <div class="row">
            <div class="col-lg-3">
              <div class="suppoter_container_title">
                <h4>Donors</h4>
              </div>
            </div>
            <div class="col-lg-9">
              <div class="suppoter_container_img">
                <img src="../assets/companyun.svg" alt="companyun" />
                <img src="../assets/companyun.svg" alt="companyun" />
                <img src="../assets/companyun.svg" alt="companyun" />
                <img src="../assets/companyun.svg" alt="companyun" />
              </div>
            </div>
          </div>
          <div class="row mt-5">
            <div class="col-lg-3">
              <div class="suppoter_container_title">
                <h4>Local NGOs</h4>
              </div>
            </div>
            <div class="col-lg-9">
              <div class="suppoter_container_img">
                <img src="../assets/companyun.svg" alt="companyun" />
                <img src="../assets/companyun.svg" alt="companyun" />
                <img src="../assets/companyun.svg" alt="companyun" />
                <img src="../assets/companyun.svg" alt="companyun" />
              </div>
              </div>
            </div>
          </div>
          <div class="row mt-5">
            <div class="col-lg-3">
              <div class="suppoter_container_title">
                <h4>UN Ageenci</h4>
              </div>
            </div>
            <div class="col-lg-9">
              <div class="suppoter_container_img">
                <img src="../assets/companyun.svg" alt="companyun" />
                <img src="../assets/companyun.svg" alt="companyun" />
                <img src="../assets/companyun.svg" alt="companyun" />
                <img src="../assets/companyun.svg" alt="companyun" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- end supporter -->
  </div>
</template>

<script>
import FeedBack from "@/components/home/FeedBack.vue";
export default {
  components: { FeedBack },
  name: "HomeView",
  data() {
    return {
      slides: [
        {
          id: 1,
          src: require("/src/assets/slider_Avatar.png"),
          src_star: require("/src/assets/Slide_Star.svg"),
          src_slider: require("/src/assets/slider.svg"),
          desc: " “Duis consectetur feugiat auctor. Morbi nec enim luctus, feugiat arcu id, ultricies ante. Duis vel massa eleifend, porta est non, feugiat metus.” ",
          name: "Marvin McKinney",
          address: "Home Seller , USA",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
// start home
.home {
  font-family: DMSans-R;
  .hero {
    background-color: #f8faff;
    &_text {
      padding-top: 100px;
      &_title {
        max-width: 560px;
        margin-top: 0px;
        margin-bottom: 24px;
        color: #2d3958;
        font-size: 64px;
        line-height: 1.07;
        font-family: DMSans-B;
        letter-spacing: -0.03em;
        margin: auto;
        margin-bottom: 24px;
      }
      &_desc {
        max-width: 540px;
        color: #7b88a8;
        font-size: 18px;
        line-height: 1.45;
        margin: auto;
        margin-bottom: 24px;
      }
      &_bottom {
        display: grid;
        place-items: center;
        text-transform: capitalize;
        min-height: 58px;
        padding-right: 32px;
        padding-left: 32px;
        transition: box-shadow 300ms ease, background-color 300ms ease;
        font-size: 16px;
        font-family: DMSans-B;
        text-align: center;
        background-color: #6a35ff;
        color: #fff;
        width: fit-content;
        margin: auto;
        &:hover {
          background-color: #5a27e7;
          box-shadow: 8px 8px 20px 0 rgb(106 53 255 / 32%);
        }
      }
    }
    &_photo {
      background-image: url("../assets/hero_background.svg");
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;
      &_Component {
        position: absolute;
        left: 0%;
        top: -20%;
        right: auto;
        bottom: auto;
        z-index: 5;
      }
      &_dashboard {
        width: 100%;
        max-width: 750px;
        border-radius: 24px;
        box-shadow: 14px 14px 55px 0 rgb(188 196 218 / 14%);
        -webkit-perspective: 1500px;
        perspective: 1500px;
        -webkit-perspective-origin: 50% 50%;
        perspective-origin: 50% 50%;
        margin-top: 45px;
      }
      &_Component1 {
        position: absolute;
        left: auto;
        top: -20%;
        right: 0%;
        bottom: auto;
        width: 100%;
        max-width: 200px;
      }
    }
  }
  .services {
    background-color: #fff;
    padding-top: 100px;
    padding-bottom: 100px;
    > .container {
      h3 {
        margin-top: 0px;
        margin-bottom: 20px;
        font-family: Manrope, sans-serif;
        color: #121f3e;
        font-size: 48px;
        line-height: 53px;
        font-family: DMSans-B;
        letter-spacing: -0.03em;
      }
      p {
        margin-bottom: 50px;
        color: #96a0b5;
        font-size: 16px;
        line-height: 32px;
        font-family: DMSans-M;
        width: 90%;
        margin: 0 auto 50px;
      }
    }
    .services_container {
      background-color: #fff;
      box-shadow: 0px 0px 10px 0px rgb(1 65 245 / 12%);
      transition: background 0.7s, border 0.5s, border-radius 0.5s,
        box-shadow 0.5s;
      margin: 10px 10px 10px 10px;
      padding: 30px 5px 30px 5px;
      border-radius: 25px 25px 25px 25px;
      transition: transform 950ms;
      &:hover {
        transform: translateY(-20px);
        box-shadow: 0px 0px 10px 0px rgb(1 65 245 / 12%);
      }
      width: 100%;
      &_img {
        img {
          width: 80px;
          margin-bottom: 10px;
        }
      }
      &_text {
        h4 {
          margin-top: 8px;
          margin-bottom: 10px;
          font-size: 16px;
          line-height: 24px;
          font-weight: 700;
          letter-spacing: -0.03em;
        }
      }
    }
  }
  .aboutus {
    padding-top: 10px;
    padding-bottom: 100px;
    font-family: DMSans-R;
    &_textside {
      text-align: left;
      display: flex;
      flex-direction: column;
      justify-content: center;
      height: 100%;
      padding: 20px;
      &_heading {
        margin-top: 20px;
        margin-bottom: 24px;
        font-size: 48px;
        line-height: 1.08;
        font-weight: 500;
        letter-spacing: -0.03em;
        text-transform: capitalize;
        font-family: DMSans-B;
      }
      &_desc {
        font-size: 18px;
        line-height: 1.45;

        margin-bottom: 10px;
        color: #7b88a8;
      }
      &_link {
        text-transform: capitalize;
        color: #6a35ff;
        font-size: 18px;
        font-family: DMSans-M;
        img {
          margin-left: 10px;
        }
      }
    }
  }
  .feedback {
    font-family: DMSans-R;
    h3 {
      margin-top: 0px;
      margin-bottom: 0px;
      font-family: Manrope, sans-serif;
      color: #121f3e;
      font-size: 40px;
      line-height: 53px;
      font-family: DMSans-B;
      letter-spacing: -0.03em;
    }
    p {
      margin-bottom: 20px;
      color: #96a0b5;
      font-size: 16px;
      line-height: 32px;
      font-family: DMSans-M;
    }
  }
  .suppoter {
    padding-top: 100px;
    padding-bottom: 100px;
    h2 {
      margin-top: 0;
      margin-bottom: 40px;
      font-family: Manrope, sans-serif;
      color: #121f3e;
      font-size: 40px;
      line-height: 53px;
      font-family: DMSans-B;
      letter-spacing: -0.03em;
    }
    &_container {
      &_title {
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;

        h4 {
          color: #4d7ef1;
          font-size: 30px;
          line-height: 53px;
          font-family: DMSans-M;
          letter-spacing: -0.03em;
          padding: 20px;
        }
        &::after {
          content: "";
          position: absolute;
          right: 0;
          top: 0;
          width: 3px;
          height: 100%;
          background-color: #4d7ef1;
        }
      }
      &_img {
        img {
          width: 25%;
        }
      }
    }
  }
}
</style>