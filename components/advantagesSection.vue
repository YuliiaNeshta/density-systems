<template>
  <section class="advantages">
    <h3 class="advantages__title title">
      Для чего нужна CRM<span class="orange-symbol">?</span>
    </h3>
    <div class="advantages__wrapper">
      <div class="advantages__item advantages-item">
        <div class="advantages-item__img">
          <img src="@/assets/images/phone.png" alt="" />
        </div>
        <p class="advantages-item__title">Автоматизируйте процессы</p>
        <p class="advantages-item__text">
          Товарищи! дальнейшее развитие различных форм деятельности требуют
          определения
        </p>
      </div>
      <div class="advantages__item advantages-item">
        <div class="advantages-item__img">
          <img src="@/assets/images/star.png" alt="" />
        </div>
        <p class="advantages-item__title">
          Нивилируйте влияние человеческого фактора
        </p>
        <p class="advantages-item__text">
          Товарищи! дальнейшее развитие различных форм деятельности требуют
          определения
        </p>
      </div>
      <div class="advantages__item advantages-item">
        <div class="advantages-item__img">
          <img src="@/assets/images/sms.png" alt="" />
        </div>
        <p class="advantages-item__title">Не теряйте ни одного покупателя</p>
        <p class="advantages-item__text">
          Товарищи! дальнейшее развитие различных форм деятельности требуют
          определения
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss">
.advantages {
  padding: 50px 0px;
  @media screen and (max-width: 769px) {
    padding-bottom: 0px;
  }
  &__title {
    margin-bottom: 100px;
    @media screen and (max-width: 769px) {
      margin-bottom: 60px;
    }
  }

  &__wrapper {
    display: flex;
    align-items: center;
    @media screen and (max-width: 992px) {
      flex-wrap: wrap;
      justify-content: center;
    }
  }

  &__item {
  }
}
.advantages-item {
  min-height: 280px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-end;
  height: 100%;
  @media screen and (max-width: 992px) {
    max-width: 450px;
    margin-bottom: 60px;
    &:last-child {
      margin-bottom: 0px;
    }
  }
  &__img {
    margin-bottom: 30px;
    max-height: 130px;
    flex: 1 1 auto;
    @media screen and (max-width: 769px) {
      margin-bottom: 45px;
    }
    @media screen and (max-width: 475px) {
      max-height: 100px;
    }
    img {
      max-width: 100%;
      vertical-align: middle;
      display: inline-block;
    }
  }

  &__title {
    font-weight: 700;
    font-size: 24px;
    line-height: 28px;
    text-align: center;
    color: #000000;
    margin-bottom: 15px;
    max-width: 370px;
    @media screen and (max-width: 769px) {
      margin-bottom: 20px;
    }
  }

  &__text {
    text-align: center;
    margin-top: auto;
  }
}
</style>
