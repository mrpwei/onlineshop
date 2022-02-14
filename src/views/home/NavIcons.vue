<template>
  <div class="icons">
    <div v-for="item in iconList" :key="item.href" class="icons__item">
      <svg class="icon icons__item__img" aria-hidden="true">
        <use :xlink:href="item.href"></use>
      </svg>
      <p class="icons__item__desc">{{ item.title }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavIcons',
  setup() {
    const iconList = [
      {
        href: '#icon-rouzhidongpin',
        title: '肉制冻品',
      },
      {
        href: '#icon-yuzhicaipin',
        title: '预制菜品',
      },
      {
        href: '#icon-haixianshuichan',
        title: '海鲜水产',
      },
      {
        href: '#icon-canchuyongpin',
        title: '餐厨用品',
      },
      {
        href: '#icon-yingyangzaocan',
        title: '营养早餐',
      },
      {
        href: '#icon-yangshengchadao',
        title: '养生茶道',
      },
      {
        href: '#icon-mimianliangyou',
        title: '米面粮油',
      },
      {
        href: '#icon-jiagongtiaoli',
        title: '加工调理',
      },
      {
        href: '#icon-shengxianshuiguo',
        title: '生鲜水果',
      },
      {
        href: '#icon-zhongwaimingjiu',
        title: '中外名酒',
      },
      {
        href: '#icon-xiuxianyinpin',
        title: '休闲饮品',
      },
      {
        href: '#icon-xiawucha',
        title: '下午茶',
      },
      {
        href: '#icon-jingpinmeizhuang',
        title: '精品美妆',
      },
      {
        href: '#icon-xinpinshangjia',
        title: '新品上架',
      },
      {
        href: '#icon-huiyuanyonghu',
        title: '会员用户',
      },
      {
        href: '#icon-shequdianpu',
        title: '社区店铺',
      },
      {
        href: '#icon-zhoubianyou',
        title: '周边游',
      },
    ]
    return {
      iconList,
    }
  },
}
</script>

<style lang="scss" scoped>
@import '../../style/variables.scss';
.icons {
  display: flex;
  flex-wrap: wrap;
  padding-top: 0.1rem;
  background-color: #fff;
  &__item {
    width: 20%;
    &__img {
      display: block;
      margin: 0 auto;
      font-size: 0.4rem;
    }
    &__desc {
      text-align: center;
      color: $content-fontcolor;
      font-size: 0.12rem;
      transform: scale(0.9, 0.9);
      transform-origin: center top;
    }
  }
}
</style>
