<template>
  <div class="scope">
    <div class="scope__row">
      <div class="scope__content">
        <p class="scope__title">Создавайте таблицы</p>
        <p class="scope__text">
          Не подстраивайтесь под разработчика, а создавайте свои таблицы или
          редактируйте существующие
        </p>
      </div>
      <div class="scope__img">
        <img src="@/assets/images/screen-3.png" alt="" />
      </div>
    </div>
    <div class="scope__row">
      <div class="scope__img">
        <img src="@/assets/images/screen-3.png" alt="" />
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
  }

  &__content {
    font-size: 16px;
    line-height: 24px;
    letter-spacing: 0.015em;
    color: #000000;
    max-width: 475px;
  }

  &__title {
    font-weight: 900;
    font-size: 36px;
    line-height: 42px;
    color: #5056e4;
    margin-bottom: 20px;
  }

  &__text {
  }

  &__img {
  }
}
</style>
