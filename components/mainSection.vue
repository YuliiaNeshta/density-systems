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
          <button class="header__btn btn btn-mobile" @click="showModal">
            Консультация
          </button>
        </div>
        <div class="main__img">
          <img src="@/assets/images/main-img.png" alt="" />
        </div>
      </div>
      <base-modal
        v-if="isFormPopupVisible"
        @closePopup="closePopup"
      ></base-modal>
    </div>
  </div>
</template>

<script>
import baseHeader from './baseHeader'
import BaseModal from './baseModal'
export default {
  components: { baseHeader, BaseModal },
  data() {
    return {
      isFormPopupVisible: false,
    }
  },
  methods: {
    showModal() {
      this.isFormPopupVisible = true
    },
    closePopup() {
      this.isFormPopupVisible = false
    },
  },
}
</script>

<style lang="scss">
.btn-mobile {
  display: none;
  @media screen and (max-width: 481px) {
    display: block;
    margin-top: 20px;
  }
}
.main {
  background-image: url('~@/assets/images/bg.png');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center center;
  padding: 0px 0px 50px 0px;
  &__row {
    display: flex;
    align-items: center;
    @media screen and (max-width: 1024px) {
      flex-direction: column-reverse;
    }
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
    @media screen and (max-width: 475px) {
      font-size: 32px;
      line-height: 38px;
      margin-bottom: 30px;
    }
  }

  &__text {
    font-size: 24px;
    line-height: 28px;
    color: #000000;
    margin-bottom: 28px;
    span {
      font-weight: 900;
    }
    @media screen and (max-width: 475px) {
      font-size: 20px;
      line-height: 23px;
      margin-bottom: 40px;
    }
  }

  &__btn {
    border: 1px solid #5056e4;
    box-sizing: border-box;
    color: #5056e4;
    align-self: flex-start;
    background-color: #fff;
    transition: all 0.3s ease 0s;
    &:hover {
      border: 1px solid #5056e4;
      color: #fff;
      background-color: #5056e4;
    }
  }

  &__img {
    @media screen and (max-width: 992px) {
      height: 495px;
      img {
        width: 100%;
        height: 100%;
        object-fit: contain;
      }
    }
    @media screen and (max-width: 475px) {
      max-width: 415px;
      height: auto;
      img {
        width: 100%;
        object-fit: cover;
      }
    }
  }
}
</style>
