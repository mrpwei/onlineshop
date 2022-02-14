<template>
  <div class="wrapper">
    <div class="search">
      <div class="search__box">
        <div class="iconfont searchicon">&#xe752;</div>
        <input v-model="input" placeholder="Type something" />
      </div>
      <div class="search__msg iconfont">&#xe62f;</div>
    </div>
    <div class="banner">
      <img
        src="https://m15.360buyimg.com/mobilecms/s1062x420_jfs/t1/110445/25/22491/530626/6203936fE199b79d5/e4855fcc3ea50b84.png!cr_1053x420_4_0!q70.jpg"
        alt="banner"
      />
    </div>
    <NavIcons />
    <Shops />
  </div>
  <Docker />
</template>

<script>
import NavIcons from './NavIcons.vue'
import Shops from './Shops.vue'
import Docker from './Docker.vue'
export default {
  name: 'Home',
  components: {
    NavIcons,
    Shops,
    Docker,
  },
}
</script>

<style lang="scss" scoped>
@import '../../style/variables.scss';
.wrapper {
  overflow-y: auto;
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0.5rem;
  background-color: #eee;
  padding-bottom: 0.2rem;
}
.search {
  display: flex;
  align-items: center;
  position: relative;
  top: 0.15rem;
  padding: 0 0.1rem;
  // background-color: red;
  height: 0.3rem;
  &__box {
    height: 100%;
    margin-right: 0.1rem;
    border-radius: 0.02rem;
    padding: 0 0.05rem;
    flex: 1;
    display: flex;
    align-items: center;
    background-color: #eee;
  }
  input {
    flex: 1;
    margin-right: 0.15rem;
    border: none;
    background-color: transparent;
  }
  input:focus {
    outline: none;
  }
  .iconfont {
    font-size: 0.24rem;
    color: $content-fontcolor;
  }
  .searchicon {
    font-size: 0.14rem;
  }
}
.banner {
  margin-top: 0.2rem;
  //防止图片加载慢引起的抖动
  height: 0;
  overflow: hidden;
  padding-bottom: 40%;
  img {
    width: 100%;
  }
}
</style>
