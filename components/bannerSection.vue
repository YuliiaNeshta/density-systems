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
  background-size: contain;
  background-position: center center;
  filter: drop-shadow(0px 4px 20px rgba(0, 0, 0, 0.15));
  border-radius: 15px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 70px;

  &__content {
    max-width: 443px;
    color: #fff;
  }

  &__title {
    font-weight: 900;
    font-size: 36px;
    line-height: 42px;
    margin-bottom: 24px;
  }

  &__text {
    margin-bottom: 24px;
    span {
      font-weight: 900;
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
  }
}
</style>
