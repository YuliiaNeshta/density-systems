<template>
  <transition name="fade">
    <div class="modal-mask">
      <div class="modal-logo">
        <img src="@/assets/images/logo.svg" alt="" />
      </div>
      <div class="modal-wrapper">
        <div class="modal-container">
          <img
            class="modal-close"
            src="@/assets/images/close.svg"
            alt="Close"
            @click="closePopup"
          />
          <p class="modal-header">
            Введите ваши данные, мы свяжемся с вами в течение 30 минут
          </p>
          <div class="modal-body">
            <slot name="body">
              <form class="modal-form" @submit.prevent="onSubmit">
                <label for="" class="modal-label">Номер телефона</label>
                <input
                  type="number"
                  class="modal-form__input"
                  v-model="mobile"
                />
                <label for="" class="modal-label">E-mail</label>
                <input type="email" class="modal-form__input" v-model="email" />
                <button class="modal-button btn">Отправить</button>
              </form>
            </slot>
            <p class="modal-text">
              Нажимая на кнопку, вы даете согласие на обработку персональных
              данных и соглашаетесь c политикой конфиденциальности
            </p>
          </div>
        </div>
      </div>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'baseModal',
  data() {
    return {
      mobile: '',
      email: '',
    }
  },
  methods: {
    closePopup() {
      this.$emit('closePopup')
    },
    onSubmit() {
      const formData = {
        mobile: this.mobile,
        email: this.email,
      }
      console.log(formData)
    },
    // resetValue() {
    //   ;(this.name = ''), (this.mobile = ''), (this.email = '')
    // },
  },
}
</script>

<style lang="scss">
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}
.fade-enter,
.fade-leave-to {
  opacity: 0;
}

.modal-label {
  font-weight: 500;
  font-size: 16px;
  line-height: 19px;
  color: #ffffff;
  margin-bottom: 6px;
  display: block;
  align-self: flex-start;
}

.modal-logo {
  margin-bottom: 30px;
  @media screen and (max-width: 779px) {
    display: none;
  }
}

.modal-text {
  font-weight: 500;
  font-size: 16px;
  line-height: 19px;
  text-align: center;
  color: #ffffff;
  @media screen and (max-width: 779px) {
    font-size: 14px;
    line-height: 16px;
  }
}

.header {
  font-weight: 300;
  font-size: 24px;
  line-height: 29px;
}

.modal-form {
  display: flex;
  flex-direction: column;
  max-width: 417px;
  width: 100%;
  margin: 0 auto;
  justify-content: center;
  align-items: center;

  &__input {
    background: rgba(255, 255, 255, 0.4);
    backdrop-filter: blur(40px);
    border-radius: 15px;
    border: 0;
    margin-bottom: 20px;
    padding: 20px;
    height: 60px;
    max-width: 417px;
    width: 100%;
    font-weight: 500;
    font-size: 16px;
    line-height: 19px;
    color: #333;

    &:focus {
      outline: none;
    }
    &::placeholder {
      font-size: 16px;
      line-height: 20px;
    }
  }
}

.modal-header {
  text-align: center;

  margin: 0 auto;
  max-width: 444px;
  font-size: 24px;
  line-height: 28px;
  text-align: center;
  color: #ffffff;
  font-weight: 700;
  @media screen and (max-width: 769px) {
    font-size: 20px;
    line-height: 23px;
    margin-bottom: 20px;
  }
}

.modal-button {
  margin-bottom: 30px;
  background-color: #5056e4;
  color: #fff;
  transition: all 0.3s ease 0s;
  border: 1px solid #5056e4;
  max-width: 202px;
  &:hover {
    border: 1px solid #5056e4;
    color: #5056e4;
    background: transparent;
  }
}

.modal-mask {
  position: fixed;

  z-index: 9998;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    138.75deg,
    #5e5e5e 3.03%,
    rgba(0, 0, 0, 0) 100.78%
  );
  backdrop-filter: blur(20px);
  transition: opacity 0.3s ease;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.modal-close {
  position: absolute;
  top: 20px;
  right: 20px;
  cursor: pointer;
  // @include for-mobile {
  //   top: 25px;
  //   right: 25px;
  // }
  @media screen and (max-width: 769px) {
    top: 10px;
    right: 10px;
  }
}

.modal-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: all 0.3s ease 0s;
  @media screen and (max-width: 769px) {
    margin: 10px;
    overflow-y: scroll;
  }
}

.modal-container {
  width: 739px;
  margin: 0px auto;
  padding: 40px 115px;
  background: rgba(255, 255, 255, 0.5);
  backdrop-filter: blur(40px);
  border-radius: 20px;
  transition: all 0.3s ease;
  position: relative;
  // @include for-tablet {
  //   width: 450px;
  // }
  // @include for-mobile {
  //   width: 100vw;
  //   padding: 60px 10px;
  // }
  @media screen and (max-width: 769px) {
    width: 100%;
    max-width: 420px;
    padding: 50px 8px;
  }
}

.modal-body {
  margin: 20px 0;
}
</style>
