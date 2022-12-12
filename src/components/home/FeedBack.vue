
<template>
  <div class="position-relative">
    <swiper class="swiper" :options="swiperOption">
      <swiper-slide v-for="(item,index) in numbers" :key="index">
        <div class="slide">
          <img
            class="img-fluid slide_img"
            :src="feedbacks.src"
            alt="slider_Avatar"
          />
          <p>
            {{ feedbacks.desc }}
          </p>
          <div class="slide_evaltion">
            <h3>{{ feedbacks.name }}</h3>
            <span>{{ feedbacks.address }}</span>
            <div class="slide_evaltion_star">
              <img src="../../assets/Slide_Star.svg" alt="Slide_Star" />
              <img src="../../assets/Slide_Star.svg" alt="Slide_Star" />
              <img src="../../assets/Slide_Star.svg" alt="Slide_Star" />
              <img src="../../assets/Slide_Star.svg" alt="Slide_Star" />
              <img src="../../assets/Slide_Star.svg" alt="Slide_Star" />
            </div>
          </div>
          <img class="slide_icon" :src="feedbacks.src_slider" alt="slider" />
        </div>
      </swiper-slide>
    </swiper>
    <div class="swiper-button-prev" slot="button-prev"></div>
    <div class="swiper-button-next" slot="button-next"></div>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";

export default {
  name: "feedback",
  props: ["feedbacks"],
  title: "Loop mode with multiple slides per group",
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      numbers: [1, 2, 3, 4, 5, 6],
      swiperOption: {
        slidesPerView: 3,
        spaceBetween: 30,
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
        breakpoints: {
          1370: {
            slidesPerView: 3,
            spaceBetween: 40,
          },
          1024: {
            slidesPerView: 3,
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
.swiper-container {
  height: 500px;
}
.slide {
  position: relative;
  height: 80%;
  padding: 30px;
  border-radius: 8px;
  background-color: #fff;
  box-shadow: 23px 23px 56px 0 rgb(0 0 0 / 5%);
  &_img {
    display: flex;
    object-fit: cover;
    overflow: hidden;
    width: 62px;
    height: 62px;
    margin-bottom: 32px;
    border-radius: 100px;
    background-color: #e5ebf0;
  }
  p {
    margin-bottom: 0px;
    color: #96a0b5;
    font-size: 16px;
    line-height: 32px;
    font-family: DMSans-M;
    text-align: left;
  }
  &_evaltion {
    text-align: left;
    margin-top: 20px;
    h3 {
      margin-bottom: 4px;
      color: #121f3e;
      font-size: 16px;
      font-family: DMSans-B;
    }
  }
  &_icon {
    position: absolute;
    left: auto;
    top: 8%;
    right: 8%;
    bottom: auto;
  }
}
.swiper-button-next,
.swiper-button-prev {
  width: 36px;
  height: 36px;
  border-radius: 50%;
  background-color: #013299;
}
.swiper-button-prev:after,
.swiper-button-next:after {
  font-size: 16px;
  color: #fff;
}
.swiper-button-next {
  right: -44px;
  @media (max-width: 991px) {
    right: -2px;
  }
}
.swiper-button-prev {
  left: -44px;
  @media (max-width: 991px) {
    left: -2px;
  }
}

.swiper-slide__content {
  height: 300px;
}
</style>