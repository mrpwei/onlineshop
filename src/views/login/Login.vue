<template>
  <div class="wrapper">
    <div class="login__header">
      <span class="login__header__help">帮助中心</span>
      <span class="login__header__language">切换语言</span>
    </div>
    <div class="login__body">
      <h1 class="login__body__avatar">mrpwei</h1>
      <div class="login__body__desc">登录账号以享受更多服务</div>
      <div class="login__body__form">密码登录</div>
      <div class="login__body__input">
        <input type="text" placeholder="请输入用户名/手机号" />
      </div>
      <div class="login__body__input">
        <input type="password" placeholder="请输入密码" />
      </div>
      <div class="login__body__links">
        <span class="login__links__forget">忘记密码</span> |
        <span class="login__links__register">立即注册</span>
      </div>
      <div class="login__body__button">
        <button @click="handleLogin">登录</button>
      </div>
    </div>
    <div class="login__footer">
      <a href="www.bing.com" target="_blank">隐私政策</a>
    </div>
  </div>
</template>

<script>
import { useRouter } from 'vue-router'
export default {
  name: 'Login',
  setup() {
    const router = useRouter()
    const handleLogin = () => {
      localStorage.isLogin = true
      router.push({ name: 'Home' })
    }
    return { handleLogin }
  },
}
</script>

<style lang="scss" scoped>
@import '../../style/variables.scss';
.wrapper {
  display: flex;
  flex-direction: column;
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  overflow: hidden; //为什么不设会滚动?
}

.login__header {
  height: 0.52rem;
  width: 100%;
  display: flex;
  align-items: center;
  color: $content-gray;
  padding-left: 2.2rem;
  &__language {
    padding-left: 0.2rem;
  }
}
.login__body {
  display: flex;
  flex-direction: column;
  flex: 1;
  &__avatar {
    text-align: center;
    color: #2ad181;
  }
  &__desc {
    height: 0.4rem;
    text-align: center;
  }
  &__form {
    height: 0.6rem;
    line-height: 0.6rem; //用百分比无效
    text-align: center;
    font-size: 0.16rem;
  }
  &__input {
    margin: 0.05rem 0.3rem;
    padding: 0 0.1rem;
    height: 0.4rem;
    background-color: #f7f8fa;
    border-radius: 0.05rem;
    input {
      outline: none;
      border: none;
      width: 100%;
      height: 100%;
      padding: 0;
      background-color: #f7f8fa;
      &::placeholder {
        color: $placeholder;
      }
    }
  }
  &__links {
    margin-left: 0.3rem;
    margin-top: 0.05rem;
    font-size: 0.12rem;
    color: $content-gray;
  }
  &__button {
    margin: 0.4rem 0.3rem;
    button {
      border: none;
      width: 100%;
      height: 0.4rem;
      border-radius: 0.05rem;
      color: #fff;
      background-color: #2ad181;
    }
  }
}
.login__footer {
  height: 0.26rem;
  text-align: center;
  padding: 0.6rem 0.4rem;
}
</style>
