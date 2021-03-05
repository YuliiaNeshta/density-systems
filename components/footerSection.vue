<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__wrapper">
        <div class="footer__row">
          <a href="tel:+380639999999" class="footer__tel footer__link"
            >+38 (063) 999 99 99</a
          >
          <a
            href="mailto:destiny.systems@gmail.com"
            class="footer__mail footer__link"
            >destiny.systems@gmail.com</a
          >
        </div>
        <div class="footer__row">
          <div class="footer__logo">
            <img src="@/assets/images/logo.svg" alt="" />
          </div>
          <p class="footer__c">2020 Все права защищены</p>
        </div>
        <div class="footer__row">
          <div class="footer__social">
            <a href="#" class="footer__link">
              <img src="@/assets/images/facebook.svg" alt="" />
            </a>
            <a href="#" class="footer__link">
              <img src="@/assets/images/facebook.svg" alt="" />
            </a>
            <a href="#" class="footer__link">
              <img src="@/assets/images/facebook.svg" alt="" />
            </a>
          </div>
          <a href="#" class="btn footer__btn">Начать бесплатно</a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {}
</script>

<style lang="scss">
.footer {
  position: relative;
  margin-top: 100px;
  background-image: url('~@/assets/images/footer.svg');
  background-repeat: no-repeat;
  background-size: cover;
  padding: 90px 0px;
  background-position: center center;
  &__wrapper {
    display: flex;
    justify-content: space-between;
  }
  &__link {
    color: #fff;
    margin-bottom: 23px;
  }

  &__row {
    flex: 1 1 33.333%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  &__social {
    margin-bottom: 26px;
    align-self: flex-end;
    text-align: right;
  }
  &__link {
    display: inline-block;
    margin-right: 15px;
  }
  &__logo {
    margin-bottom: 30px;
  }
  &__btn {
    border: 1px solid #fff;
    color: #fff;
    text-align: center;
    align-self: flex-end;
    transition: all 0.3s ease 0s;
    &:hover {
      background-color: #fff;
      color: #000;
    }
  }
  &__c {
    text-align: center;
    color: #ffffff;
  }
}
</style>
