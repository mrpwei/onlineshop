<template>
  <div class="docker">
    <div
      v-for="(item, index) in dockerList"
      :key="item.icon"
      :class="{ docker__item: true, 'docker__item--active': index === 0 }"
      class="docker__item docker__item--active"
    >
      <div class="iconfont" v-html="item.icon" />
      <div class="docker__item__title">{{ item.title }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Docker',
  setup() {
    const dockerList = [
      { icon: '&#xe663;', title: '首页' },
      { icon: '&#xe73d;', title: '购物车' },
      { icon: '&#xe693;', title: '消息' },
      { icon: '&#xe607;', title: '我的' },
    ]
    return { dockerList }
  },
}
</script>

<style lang="scss" scoped>
@import '../../style/variables.scss';
.docker {
  display: flex;
  position: absolute;
  box-sizing: border-box; //todo
  left: 0;
  bottom: 0;
  width: 100%;
  height: 0.5rem;
  border-top: 1px solid #ee4d2d;
  // background-color: green;
  &__item {
    flex: 1;
    text-align: center;
    margin: 0.06rem 0 0 0;
    color: $content-fontcolor;
    .iconfont {
      font-size: 0.24rem;
    }
    &__title {
      //需要10px的字体，但是默认最小显示12px，则可以这样设置
      font-size: 0.2rem;
      transform: scale(0.5, 0.5);
      transform-origin: center top;
    }
    &--active {
      color: #ee4d2d;
    }
  }
}
</style>
