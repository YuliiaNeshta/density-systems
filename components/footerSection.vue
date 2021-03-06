<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__wrapper">
        <div class="footer__row footer__contacts footer__row--contacts">
          <a href="tel:+380639999999" class="footer__tel footer__link"
            >+38 (063) 999 99 99</a
          >
          <a
            href="mailto:destiny.systems@gmail.com"
            class="footer__mail footer__link"
            >destiny.systems@gmail.com</a
          >
        </div>
        <div class="footer__row footer__row--logo">
          <div class="footer__logo">
            <img src="@/assets/images/logo.svg" alt="" />
          </div>
          <p class="footer__c">2020 Все права защищены</p>
        </div>
        <div class="footer__row footer__row--social">
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
        <p class="footer__c--mobile">2020 Все права защищены</p>
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
  background-position: top center;
  &__wrapper {
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    @media screen and (max-width: 769px) {
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }
  }

  &__link {
    color: #fff;
    margin-bottom: 23px;
  }
  &__tel {
    background-image: url('~@/assets/images/call.svg');
    padding-left: 40px;
    background-repeat: no-repeat;
    background-position: center left;
  }
  &__mail {
    background-image: url('~@/assets/images/mail.svg');
    padding-left: 40px;
    background-repeat: no-repeat;
    background-position: center left;
  }

  &__row {
    flex: 1 1 33.333%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    @media screen and (max-width: 769px) {
      flex: 1 1 100%;
    }
    &--logo {
      @media screen and (max-width: 769px) {
        order: 1;
      }
    }
    &--contacts {
      @media screen and (max-width: 769px) {
        order: 2;
      }
    }
    &--social {
      @media screen and (max-width: 769px) {
        order: 3;
      }
    }
  }
  &__contacts {
    align-items: flex-start;
  }
  &__social {
    margin-bottom: 26px;
    align-self: flex-end;
    text-align: right;
    height: 25px;
    @media screen and (max-width: 769px) {
      align-self: initial;
    }
  }
  &__link {
    display: inline-block;
    margin-right: 15px;
    @media screen and (max-width: 769px) {
      &:last-child {
        margin-right: 0px;
      }
    }
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
    margin-bottom: 24px;
    @media screen and (max-width: 769px) {
      align-self: initial;
    }
    &:hover {
      background-color: #fff;
      color: #000;
    }
  }
  &__c {
    text-align: center;
    color: #ffffff;
    &--mobile {
      display: none;
      @media screen and (max-width: 769px) {
        text-align: center;
        color: #ffffff;
        display: block;
        order: 4;
        margin-top: 70px;
      }
    }
    @media screen and (max-width: 769px) {
      display: none;
    }
  }
}
</style>
