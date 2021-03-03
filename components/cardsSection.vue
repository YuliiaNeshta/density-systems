<template>
  <section class="plans">
    <div class="container">
      <div class="plans__cards">
        <h3 class="plans__title title">Выберите свою версию</h3>
        <p class="plans__descr">
          Работайте с комфортом — выберите ту версию, в которой вам будет
          работать удобнее всего
        </p>
        <div class="card__wrapper">
          <div class="card">
            <div class="card__image">
              <img src="@/assets/images/plan-1.svg" alt="" />
            </div>
            <p class="card__title">Аренда аккаунта</p>
            <p class="card__text">
              Не нужно заботиться об установке программы и ее обновлениях — все
              осуществляется на нашем сервере
            </p>
            <div class="card__hover">
              <p class="card__price">от 300 грн/мес</p>
              <a href="#" class="card__btn btn">Начать бесплатно</a>
            </div>
          </div>
          <div class="card card--margin">
            <div class="card__image">
              <img src="@/assets/images/plan-1.svg" alt="" />
            </div>
            <p class="card__title">Коробочная лицензия</p>
            <p class="card__text">
              Перенесите все бизнес-процессы в CRM систему и настройте
              безопасное локальное подключение — максимальная сохранность ваших
              данных
            </p>
            <div class="card__hover">
              <p class="card__price">от 3000 грн</p>
              <a href="#" class="card__btn btn">Начать бесплатно</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss">
.plans {
  padding-top: 250px;
  padding-bottom: 180px;

  &__cards {
  }

  &__title {
    margin-bottom: 30px;
  }

  &__descr {
    margin-bottom: 90px;
    text-align: center;
  }
}

.card {
  box-shadow: 0px 4px 28px rgba(0, 0, 0, 0.25);
  border-radius: 15px;
  max-width: 363px;
  padding: 30px 30px 60px 30px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-right: 30px;
  &--margin {
    transform: translateY(40px);
  }
  &__image {
    margin-bottom: 30px;
  }

  &__title {
    font-size: 16px;
    line-height: 19px;
    font-weight: 700;
    margin-bottom: 20px;
  }

  &__text {
    text-align: center;
    margin-bottom: 30px;
  }

  &__wrapper {
    display: flex;
    justify-content: center;
  }

  &__price {
    font-weight: 700;
    margin-bottom: 20px;
    font-size: 24px;
    line-height: 28px;
    text-align: center;
    color: #000;
    transition: all 0.3s ease 0s;
  }
  &__hover {
    &:hover {
      & .card__price {
        color: #5056e4;
      }
      & .card__btn {
        background: #4951ff;
        color: #ffffff;
      }
    }
  }

  &__btn {
    display: inline-block;
    font-size: 16px;
    line-height: 19px;
    color: #5056e4;
    min-width: 202px;
    transition: all 0.6s ease 0s;
    border-radius: 25px;
    text-align: center;
    background: #fff;
    border: 1px solid #5056e4;
  }
}
</style>
