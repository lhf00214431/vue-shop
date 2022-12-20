<template>
  <div class="wrapper">
    <img :src="user" alt="" class="wrapper__img">
    <div class="wrapper__input">
      <input
      type="text"
      class="wrapper__input__content"
      placeholder="请输入用户名"
      v-model="username"
      >
    </div>
    <div class="wrapper__input">
      <input
      type="password"
      class="wrapper__input__content"
      placeholder="请输入密码"
      v-model="password"
      >
    </div>
    <div class="wrapper__input">
      <input
      type="password"
      class="wrapper__input__content"
      placeholder="确认密码"
      v-model="ensurement"
      >
    </div>
    <div class="wrapper__register-button" @click="handleRegister">注册</div>
    <div class="wrapper__register-link" @click="handleLoginClick">已有账号去登录</div>
    <Toast v-if="show" :message="toastMessage"/>
  </div>
</template>

<script>
import { useRouter } from 'vue-router'
import { reactive, toRefs } from 'vue'
import user from '@/image/user.png'
import { post } from '@/utils/request'
import Toast, { useToastEffect } from '@/components/Toast'

const useRegisterEffect = (showToast) => {
  const router = useRouter()
  const data = reactive({ username: '', password: '', ensurement: '' })

  const handleRegister = async () => {
    try {
      const result = await post('/api/user/register',
        {
          username: data.username,
          password: data.password
        })

      if (result?.error === 0) {
        localStorage.isLogin = true
        router.push({ name: 'Home' })
      } else {
        showToast('登录失败')
        // alert('登录失败')
      }
    } catch (e) {
      showToast('请求失败')
      // alert('请求失败')
    }
  }

  const { username, password, ensurement } = toRefs(data)
  return { username, password, ensurement, handleRegister }
}
const useLoginEffect = () => {
  const router = useRouter()
  const handleLoginClick = () => {
    router.push({ name: 'Login' })
  }
  return {
    handleLoginClick
  }
}

export default {
  name: 'Register',
  components: { Toast },
  props: {
  },
  setup () {
    const { handleLoginClick } = useLoginEffect()
    const { username, password, ensurement, handleRegister } = useRegisterEffect(useToastEffect)
    return {
      user,
      handleLoginClick,
      username,
      password,
      ensurement,
      handleRegister
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
  &__register-button{
    margin: .32rem .4rem 0.16rem .4rem;
    line-height: .48rem;
    background: #0091FF;
    box-shadow: 0 .04rem .08rem rgba(0, 145, 255, 0.32);
    border-radius: .04rem;
    color: #fff;
    font-size: .16rem;
    text-align: center;
  }
  &__register-link {
    text-align: center;
    font-size: .14rem;
    color: $content-notice-font-color;
  }
}
</style>
