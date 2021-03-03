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
  padding: 120px 0px;
  &__title {
    margin-bottom: 100px;
  }

  &__wrapper {
    display: flex;
  }

  &__item {
  }
}
.advantages-item {
  flex: 1 1 33.333%;
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 100%;
  &__img {
    margin-bottom: 30px;
    flex: 1 1 auto;
  }

  &__title {
    font-weight: 700;
    font-size: 24px;
    line-height: 28px;
    text-align: center;
    color: #000000;
    margin-bottom: 15px;
  }

  &__text {
    text-align: center;
  }
}
</style>
