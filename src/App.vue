<template>
  <div>
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
      <div class="icons">
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-rouzhidongpin"></use>
          </svg>
          <p class="icons__item__desc">肉制冻品</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-yuzhicaipin"></use>
          </svg>
          <p class="icons__item__desc">预制菜品</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-haixianshuichan"></use>
          </svg>
          <p class="icons__item__desc">海鲜水产</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-canchuyongpin"></use>
          </svg>
          <p class="icons__item__desc">餐厨用品</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-yingyangzaocan"></use>
          </svg>
          <p class="icons__item__desc">营养早餐</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-yangshengchadao"></use>
          </svg>
          <p class="icons__item__desc">养生茶道</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-mimianliangyou"></use>
          </svg>
          <p class="icons__item__desc">米面粮油</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-jiagongtiaoli"></use>
          </svg>
          <p class="icons__item__desc">加工调理</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-shengxianshuiguo"></use>
          </svg>
          <p class="icons__item__desc">生鲜水果</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-zhongwaimingjiu"></use>
          </svg>
          <p class="icons__item__desc">中外名酒</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-xiuxianyinpin"></use>
          </svg>
          <p class="icons__item__desc">休闲饮品</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-xiawucha"></use>
          </svg>
          <p class="icons__item__desc">下午茶</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-jingpinmeizhuang"></use>
          </svg>
          <p class="icons__item__desc">精品美妆</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-xinpinshangjia"></use>
          </svg>
          <p class="icons__item__desc">新品上架</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-huiyuanyonghu"></use>
          </svg>
          <p class="icons__item__desc">会员用户</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-shequdianpu"></use>
          </svg>
          <p class="icons__item__desc">社区店铺</p>
        </div>
        <div class="icons__item">
          <svg class="icon icons__item__img" aria-hidden="true">
            <use xlink:href="#icon-zhoubianyou"></use>
          </svg>
          <p class="icons__item__desc">周边游</p>
        </div>
      </div>
      <div class="shops">
        <div class="shops__item">
          <img
            src="https://kaola-haitao.oss.kaolacdn.com/1c12r2jsa69_400_400.jpg?x-oss-process=image/resize,w_240,h_240/quality,q_60/format,webp/ignore-error,1"
            alt="sony"
            class="shops__item__img"
          />
          <div class="shops__item__info">
            <div>索尼</div>
            <div>月销：126</div>
          </div>
        </div>
        <div class="shops__item">
          <img
            src="https://kaola-haitao.oss.kaolacdn.com/1c12qt70k22_400_400.jpg?x-oss-process=image/resize,w_240,h_240/quality,q_60/format,webp/ignore-error,1"
            alt="dyson"
            class="shops__item__img"
          />
          <div class="shops__item__info">
            <div>戴森</div>
            <div>月销：126</div>
          </div>
        </div>
        <div class="shops__item">
          <img
            src="https://kaola-haitao.oss.kaolacdn.com/ilvm0ozg86_300_300.jpg?x-oss-process=image/resize,w_240,h_240/quality,q_60/format,webp/ignore-error,1"
            alt="puma"
            class="shops__item__img"
          />
          <div class="shops__item__info">
            <div>彪马</div>
            <div>月销：126</div>
          </div>
        </div>
        <div class="shops__item">
          <img
            src="https://kaola-haitao.oss.kaolacdn.com/ii02shtz66_300_300.jpg?x-oss-process=image/resize,w_240,h_240/quality,q_60/format,webp/ignore-error,1"
            alt="nike"
            class="shops__item__img"
          />
          <div class="shops__item__info">
            <div>耐克</div>
            <div>月销：126</div>
          </div>
        </div>
      </div>
    </div>
    <div class="docker">
      <div class="docker__item docker__item--active">
        <div class="iconfont">&#xe663;</div>
        <div class="docker__item__title">首页</div>
      </div>
      <div class="docker__item">
        <div class="iconfont">&#xe73d;</div>
        <div class="docker__item__title">购物车</div>
      </div>
      <div class="docker__item">
        <div class="iconfont">&#xe693;</div>
        <div class="docker__item__title">消息</div>
      </div>
      <div class="docker__item">
        <div class="iconfont">&#xe607;</div>
        <div class="docker__item__title">我的</div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
const input = ref('')
</script>

<style lang="scss">
@import './style/variables.scss';
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
