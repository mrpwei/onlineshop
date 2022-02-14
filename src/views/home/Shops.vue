<template>
  <div class="shops">
    <div v-for="item in shopList" :key="item.name" class="shops__item">
      <img :src="item.imgSrc" :alt="item.name" class="shops__item__img" />
      <div class="shops__item__info">
        <div>{{ item.name }}</div>
        <div>月销：{{ item.sales }}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Shops',
  setup() {
    const shopList = [
      {
        name: '索尼',
        imgSrc:
          'https://kaola-haitao.oss.kaolacdn.com/1c12r2jsa69_400_400.jpg?x-oss-process=image/resize,w_240,h_240/quality,q_60/format,webp/ignore-error,1',
        sales: 125,
      },
      {
        name: '彪马',
        imgSrc:
          'https://kaola-haitao.oss.kaolacdn.com/ilvm0ozg86_300_300.jpg?x-oss-process=image/resize,w_240,h_240/quality,q_60/format,webp/ignore-error,1',
        sales: 240,
      },
      {
        name: '耐克',
        imgSrc:
          'https://kaola-haitao.oss.kaolacdn.com/ii02shtz66_300_300.jpg?x-oss-process=image/resize,w_240,h_240/quality,q_60/format,webp/ignore-error,1',
        sales: 200,
      },
      {
        name: '戴森',
        imgSrc:
          'https://kaola-haitao.oss.kaolacdn.com/1c12qt70k22_400_400.jpg?x-oss-process=image/resize,w_240,h_240/quality,q_60/format,webp/ignore-error,1',
        sales: 12,
      },
    ]
    return { shopList }
  },
}
</script>

<style lang="scss" scoped>
.shops {
  margin-top: 0.1rem;
  &__item {
    display: flex;
    align-items: center;
    background-color: #fff;
    border-bottom: 1px solid #eee;
    padding-left: 0.1rem;
    &__img {
      height: 1rem;
      width: 1rem;
    }
    &__info {
      padding-left: 0.2rem;
      // display: flex;
    }
  }
}
</style>
