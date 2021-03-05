<template>
  <header class="header">
    <div class="header__logo">
      <img src="@/assets/images/logo.svg" alt="" />
    </div>
    <div class="header__contacts">
      <a href="tel:+380669999999" class="header__tel">+38 (066) 999 99 99</a>
      <button class="header__btn btn" @click="showModal">Консультация</button>
    </div>
    <base-modal v-if="isFormPopupVisible" @closePopup="closePopup"></base-modal>
  </header>
</template>

<script>
import baseModal from './baseModal'

export default {
  components: { baseModal },
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
.header {
  display: flex;
  justify-content: space-between;
  padding: 30px 0px;
  &__logo {
    width: 205px;
    height: 115px;
    img {
      width: 100%;
    }
  }

  &__contacts {
    display: flex;
    align-items: center;
  }

  &__tel {
    font-size: 16px;
    line-height: 19px;
    color: #ffffff;
    display: inline-block;
    margin-right: 35px;
  }

  &__btn {
    font-size: 16px;
    line-height: 19px;
    color: #ffffff;
    background: linear-gradient(92.26deg, #5056e4 14.33%, #4951ff 103.24%);
  }
}
</style>
