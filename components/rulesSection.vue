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
  padding-bottom: 200px;
  &__title {
    margin-bottom: 20px;
  }

  &__descr {
    text-align: center;
    margin-bottom: 90px;
  }
  &__img {
    display: flex;
    position: relative;
    justify-content: center;
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
  }

  & .img-main {
    position: relative;
    z-index: 5;
  }
  & .img-left {
    left: 5%;
  }
}
</style>
