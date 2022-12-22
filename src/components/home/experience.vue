<template>
  <div class="swp mt-2">
    <swiper class="swiper" :options="swiperOption">
      <swiper-slide v-for="(item, index) in numbers" :key="index">
        <div class="slide">
          <div class="experience_humanitairy_srv">
            <img
              src="../../assets/experience_humanitairy.svg"
              alt="experience humanitairy"
            />
            <div
              class="
                experience_humanitairy_srv_box
                d-flex
                align-items-center
                gap-2
              "
            >
              <h2>27</h2>
              <p>Food Security</p>
            </div>
          </div>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";
export default {
  name: "experience",
  title: "Loop mode with multiple slides per group",
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      numbers: [1, 2, 3, 4, 5, 6 ,7 ,8 ,9 , 10],
      swiperOption: {
        slidesPerView: 3,
        spaceBetween: 30,
        autoplay: {
        delay: 2000,
        disableOnInteraction: false
        },
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
        breakpoints: {
          1370: {
            slidesPerView: 5,
            spaceBetween: 40,
          },
          1024: {
            slidesPerView: 4,
            spaceBetween: 40,
          },
          768: {
            slidesPerView: 1,
            spaceBetween: 30,
          },
          640: {
            slidesPerView: 1,
            spaceBetween: 20,
          },
          320: {
            slidesPerView: 1,
            spaceBetween: 10,
          },
        },
      },
    };
  },
};
</script>
<style lang="scss" scoped>
.experience {
    padding-top: 100px;
    &_humanitairy {
      h3 {
        font-size: 48px;
        font-family: DMSans-B;
        margin-bottom: 24px;
        color: #182135;
      }
      p {
        width: 1088px;
        max-width: 100%;
        margin: auto;
        font-size: 20px;
        line-height: 32px;
        color: #627d98;
      }
      &_srv {
        width: 220px;
        height: 150px;
        background-color: #e9f9fe;
        border-radius: 0 20px 20px;
        position: relative;
        margin-top: 35.8px;
        box-shadow: 0 0 6px rgb(0 0 0 / 10%);
        img {
          position: absolute;
          top: -45px;
          left: -8.5px;
        }
        &_box {
          width: 198.58px;
          text-align: left;
          padding: 45px 45px 36px 16.4px;
          h2 {
            margin-bottom: 0;
            color: #0f609b;
            font-size: 72px;
            font-family: DMSans-B;
          }
          p {
            font-size: 24px;
            line-height: 31px;
            color: #0f609b;
            font-family: DMSans-M;
            margin: 0;
          }
        }
      }
    }
  }
</style>