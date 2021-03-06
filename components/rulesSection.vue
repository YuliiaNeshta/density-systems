<template>
  <section class="rules">
    <div class="container">
      <h2 class="rules__title title">
        CRM система по вашим правилам<span class="orange-symbol">:</span>
      </h2>
      <p class="rules__descr">Только необходимые вам отчеты и таблицы</p>
      <div class="rules__img">
        <img class="img-left" src="~/assets/images/slider-2.png" alt="" />
        <img class="img-main" src="~/assets/images/slider-1.png" alt="" />
        <img class="img-right" src="~/assets/images/slider-3.png" alt="" />
      </div>
      <!-- <div v-swiper:mySwiper="rules" class="swiper-container">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <img src="~/assets/images/slider-1.png" alt="" />
          </div>
          <div class="swiper-slide">
            <img src="~/assets/images/slider-2.png" alt="" />
          </div>
          <div class="swiper-slide">
            
          </div>
        </div>
      </div> -->
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      rules: {
        spaceBetween: 20,
        slidesPerView: 3,
      },
    }
  },
}
</script>

<style lang="scss">
.rules {
  background-image: url('~@/assets/images/bg-slider.png');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center center;
  padding: 200px 0px;
  backdrop-filter: blur(28px);
  @media screen and (max-width: 769px) {
    padding: 120px 0px;
    padding-bottom: 220px;
  }
  &__title {
    margin-bottom: 20px;
  }

  &__descr {
    text-align: center;
    margin-bottom: 90px;
    @media screen and (max-width: 769px) {
      margin-bottom: 60px;
    }
  }
  &__img {
    display: flex;
    position: relative;
    justify-content: center;
    img {
      @media screen and (max-width: 769px) {
        max-width: 300px;
      }
    }
  }
  & .img-right,
  .img-left {
    position: absolute;
    z-index: 2;
    top: 50%;
    transform: translateY(-50%);
  }

  & .img-right {
    right: 5%;
    @media screen and (max-width: 769px) {
      max-width: 180px;
      right: 47vw;
      top: auto;
      bottom: -87%;
    }
  }

  & .img-main {
    position: relative;
    z-index: 5;
  }
  & .img-left {
    left: 5%;

    @media screen and (max-width: 769px) {
      top: auto;
      bottom: -200px;
      left: 33%;
      max-width: 180px;
    }
  }
}
</style>
