<template>
  <div class="wrapper">
    <Search />
    <Banner />
    <NavIcons />
    <Shops />
  </div>
  <Docker />
</template>

<script>
import NavIcons from './NavIcons.vue'
import Shops from './Shops.vue'
import Docker from './Docker.vue'
import Banner from './Banner.vue'
import Search from './Search.vue'
export default {
  name: 'Home',
  components: {
    NavIcons,
    Shops,
    Docker,
    Banner,
    Search,
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
  background-color: #f7f8fa;
  padding-bottom: 0.2rem;
}

// .banner {
//   //防止图片加载慢引起的抖动
//   height: 0;
//   overflow: hidden;
//   padding-bottom: 40%;
//   img {
//     width: 100%;
//   }
// }
</style>
