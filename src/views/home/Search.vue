<template>
  <div class="search">
    <div class="search__wrapper">
      <div class="search__wrapper__box">
        <div class="iconfont searchicon">&#xe752;</div>
        <input v-model="input" placeholder="Type something" />
      </div>
      <div class="search__msg iconfont">&#xe62f;</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Search',
}
</script>

<style lang="scss" scoped>
@import '../../style/variables.scss';
.search {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 100;
  background-color: transparent;
  height: 0.46rem;
  width: 100%;
  display: flex;
  align-items: center;
  &__wrapper {
    display: flex;
    align-items: center;
    width: 100%;
    padding: 0 0.1rem;
    &__box {
      height: 0.32rem;
      margin-right: 0.1rem;
      border-radius: 0.02rem;
      padding: 0 0.05rem;
      flex: 1;
      display: flex;
      align-items: center;
      background-color: #f7f8fa;
      input {
        flex: 1;
        margin-right: 0.15rem;
        border: none;
        background-color: transparent;
      }
      input:focus {
        outline: none;
      }
    }
  }

  .iconfont {
    font-size: 0.24rem;
    color: #fff;
  }
  .searchicon {
    font-size: 0.14rem;
    color: $content-fontcolor;
  }
}
</style>
