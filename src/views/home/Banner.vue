<template>
  <div class="banner">
    <el-carousel height="2.08rem">
      <el-carousel-item v-for="item in bannerList" :key="item">
        <img :src="item.src" alt="banner" />
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
export default {
  name: 'Banner',
  setup() {
    const bannerList = [
      {
        index: 0,
        src: 'https://dsfs.oppo.com/archives/202202/20220214050235620a25eb480bc.jpg?_w_=1080&_h_=600&x-oss-process=image/format,webp',
      },
      {
        index: 1,
        src: 'https://dsfs.oppo.com/archives/202201/2022011204012561de8d69e7ff8.png?_w_=1080&_h_=600&x-oss-process=image/format,webp',
      },
      {
        index: 2,
        src: 'https://dsfs.oppo.com/archives/202202/20220214050222620a24ee6d2a8.jpg?_w_=1080&_h_=600&x-oss-process=image/format,webp',
      },
      {
        index: 3,
        src: 'https://dsfs.oppo.com/archives/202202/20220214050217620a2525111df.jpg?_w_=1080&_h_=600&x-oss-process=image/format,webp',
      },
      {
        index: 4,
        src: 'https://dsfs.oppo.com/archives/202202/20220214050207620a255777754.jpg?_w_=1080&_h_=600&x-oss-process=image/format,webp',
      },
    ]
    return { bannerList }
  },
}
</script>

<style lang="scss" scoped>
.banner {
  img {
    width: 100%;
  }
}
</style>
