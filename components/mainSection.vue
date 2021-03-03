<template>
  <div class="main">
    <div class="container">
      <base-header></base-header>
      <div class="main__row">
        <div class="main__content">
          <h1 class="main__title">
            CRM — время для оптимизации вашего бизнеса<span
              class="orange-symbol"
              >.</span
            >
          </h1>
          <p class="main__text">
            С помощью <span>CRM-системы от 1С</span> оптимизируем проекты любого
            масштаба
          </p>
          <button class="main__btn btn">Читать больше</button>
        </div>
        <div class="main__img">
          <img src="@/assets/images/main-img.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import baseHeader from './baseHeader'
export default {
  components: { baseHeader },
}
</script>

<style lang="scss">
.main {
  background-image: url('~@/assets/images/bg.png');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center center;
  padding: 0px 0px 50px 0px;
  &__row {
    display: flex;
    align-items: center;
  }

  &__content {
    max-width: 560px;
  }

  &__title {
    font-weight: 900;
    font-size: 48px;
    line-height: 56px;
    color: #5056e4;
    margin-bottom: 18px;
  }

  &__text {
    font-size: 24px;
    line-height: 28px;
    color: #000000;
    margin-bottom: 28px;
    span {
      font-weight: 900;
    }
  }

  &__btn {
    border: 1px solid #5056e4;
    box-sizing: border-box;
    color: #5056e4;
    align-self: flex-start;
    background-color: #fff;
  }

  &__img {
  }
}
</style>
