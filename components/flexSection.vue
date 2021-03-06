<template>
  <div class="scope">
    <div class="scope__row">
      <div class="scope__content">
        <p class="scope__title title">Создавайте таблицы</p>
        <p class="scope__text">
          Не подстраивайтесь под разработчика, а создавайте свои таблицы или
          редактируйте существующие
        </p>
      </div>
      <div class="scope__img">
        <img src="@/assets/images/screen-3.png" alt="" />
        <div class="spot-red"></div>
      </div>
    </div>
    <div class="scope__row scope__row--reverse">
      <div class="scope__img">
        <img src="@/assets/images/screen-2.png" alt="" />
        <div class="spot-green"></div>
      </div>
      <div class="scope__content">
        <p class="scope__title">Добавляйте вычисления</p>
        <p class="scope__text">
          В любое поле или таблицу можно добавить формулу для автоматического
          рассчета значения любой сложности
        </p>
      </div>
    </div>
    <div class="scope__row">
      <div class="scope__content">
        <p class="scope__title">Генерируйте документы и отчеты</p>
        <p class="scope__text">
          Автоматически оздавайте документацию и отчеты. Сокращайте количество
          ошибок в документах, надежно храните и упорядочивайте, ускоряя
          бизнес-процессы компании
        </p>
      </div>
      <div class="scope__img">
        <div class="spot-blue"></div>
        <img src="@/assets/images/screen-3.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
.scope {
  &__row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    @media screen and (max-width: 992px) {
      flex-direction: column;
      margin-bottom: 120px;
      &:last-child {
        margin-bottom: 0px;
      }
    }
    &--reverse {
      justify-content: space-around;
      @media screen and (max-width: 992px) {
        flex-direction: column-reverse;
      }
    }
  }

  &__content {
    font-size: 16px;
    line-height: 24px;
    letter-spacing: 0.015em;
    color: #000000;
    max-width: 475px;
    @media screen and (max-width: 992px) {
      margin-bottom: 60px;
    }
  }

  &__title {
    font-weight: 900;
    font-size: 36px;
    line-height: 42px;
    color: #5056e4;
    margin-bottom: 20px;
    @media screen and (max-width: 475px) {
      font-size: 24px;
      line-height: 28px;
    }
  }

  &__text {
  }

  &__img {
    position: relative;
    img {
      width: 100%;
    }
    @media screen and (max-width: 475px) {
      max-width: 300px;
      img {
        width: 100%;
      }
    }
  }
}

.spot-green {
  position: absolute;
  width: 107px;
  height: 107px;
  background: linear-gradient(90deg, #43e97b 0%, #38f9d7 100%);
  filter: blur(80px);
  z-index: -1;
  top: 60px;
  right: 60px;
}
.spot-red {
  position: absolute;
  z-index: -1;
  bottom: 118px;
  left: 74px;
  width: 107px;
  height: 107px;
  background: linear-gradient(
    90deg,
    #ff8177 0%,
    #ff867a 0%,
    #ff8c7f 21%,
    #f99185 52%,
    #cf556c 78%,
    #b12a5b 100%
  );
  filter: blur(73px);
}
.spot-blue {
  position: absolute;
  width: 107px;
  height: 107px;
  background: linear-gradient(90deg, #4facfe 0%, #00f2fe 100%);
  filter: blur(80px);
  z-index: -1;
  bottom: 60px;
  left: 29px;
  bottom: 110px;
  left: 27px;
}
</style>
