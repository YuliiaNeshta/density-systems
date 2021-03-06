<template>
  <div class="container">
    <div class="banner">
      <div class="banner__content">
        <p class="banner__title">Попробуйте бесплатно</p>
        <p class="banner__text">
          Тестируйте полную версию CRM системы
          <span>бесплатно в течение 14 дней</span>
        </p>
        <button class="banner__btn btn">Начать бесплатно</button>
      </div>
      <div class="banner__img">
        <img src="@/assets/images/banner.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
.banner {
  background-image: url('~@/assets/images/bg-banner.png');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center center;
  // filter: drop-shadow(0px 4px 20px rgba(0, 0, 0, 0.15));
  border-radius: 43px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0px 70px;
  max-height: 340px;
  @media screen and (max-width: 769px) {
    flex-direction: column;
    background-image: url('~@/assets/images/banner-mobile.png');
    border-radius: 43px;
    padding: 65px 10px;
    padding-bottom: 0px;
    max-height: none;
  }

  &__content {
    max-width: 443px;
    color: #fff;
    padding: 70px 0px;
  }

  &__title {
    font-weight: 900;
    font-size: 36px;
    line-height: 42px;
    margin-bottom: 24px;
    @media screen and (max-width: 475px) {
      font-size: 24px;
      line-height: 28px;
      margin-bottom: 20px;
    }
  }

  &__text {
    margin-bottom: 24px;
    span {
      font-weight: 900;
    }
    @media screen and (max-width: 475px) {
      margin-bottom: 20px;
    }
  }

  &__btn {
    background-color: transparent;
    border: 1px solid #fff;
    color: #fff;
    transition: all 0.3s ease 0s;
    &:hover {
      background-color: #fff;
      color: #000;
    }
  }

  &__img {
    max-width: 480px;
    @media screen and (max-width: 475px) {
      max-width: 320px;
      img {
        width: 100%;
      }
    }
  }
}
</style>
