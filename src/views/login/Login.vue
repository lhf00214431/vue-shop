<template>
  <div class="wrapper">
    <img :src="user" alt="" class="wrapper__img">
    <div class="wrapper__input">
      <input type="text" class="wrapper__input__content" placeholder="请输入手机号">
    </div>
    <div class="wrapper__input">
      <input type="text" class="wrapper__input__content" placeholder="请输入密码">
    </div>
    <div class="wrapper__login-button" @click="handleLogin">登录</div>
    <div class="wrapper__login-link">立即注册</div>
  </div>
</template>

<script>
import { useRouter } from 'vue-router'
import user from '@/image/user.png'
export default {
  name: 'LoginLogin',
  props: {
  },
  setup () {
    const router = useRouter()
    const handleLogin = () => {
      localStorage.isLogin = true
      router.push({ name: 'Home' })
    }
    return {
      user,
      handleLogin
    }
  }
}

</script>
<style lang="scss" scoped>
@import '@/style/viriables.scss';
.wrapper {
  position: absolute;
  top: 50%;
  left: 0;
  right: 0;
  transform: translateY(-50%);
  &__img {
    display: block;
    margin: 0 auto .4rem auto;
    width: .66rem;
    height: .66rem;
  }
  &__input {
    height: .48rem;
    margin: 0 .4rem .16rem .4rem;
    padding: 0 .16rem;
    background: #F9F9F9;
    border: 0.01rem solid rgba(0, 0, 0, 0.10);
    border-radius: .06rem;
    &__content {
      line-height: .48rem;
      border: none;
      outline: none;
      width: 100%;
      background: none;
      font-size: .16rem;
      color: $content-notice-font-color;
      &::placeholder {
        color: $content-notice-font-color;
      }
    }
  }
  &__login-button{
    margin: .32rem .4rem 0.16rem .4rem;
    line-height: .48rem;
    background: #0091FF;
    box-shadow: 0 .04rem .08rem rgba(0, 145, 255, 0.32);
    border-radius: .04rem;
    color: #fff;
    font-size: .16rem;
    text-align: center;
  }
  &__login-link {
    text-align: center;
    font-size: .14rem;
    color: $content-notice-font-color;
  }
}
</style>
