<template>
      <div class="position">
      <span class="iconfont position__icon">&#xe67f;</span>
      北京理工大学供方科技园2号楼10层
      <span class="iconfont position__notice">&#xe729;</span>
    </div>
    <div class="search">
      <span class="iconfont search__icon">&#xe741;</span>
      <span class="search__text">山姆会员商店优惠商品</span>
    </div>
    <div class="banner">
      <img class="banner__image" :src="banner" alt="">
    </div>
    <div class="icons">
      <div class="icons__item">
        <img :src="supermarket" alt="" class="icons__item__img">
        <p class="icons__item__desc">超市便利</p>
      </div>
      <div class="icons__item">
        <img :src="vegetableMarket" alt="" class="icons__item__img">
        <p class="icons__item__desc">菜市场</p>
      </div>
      <div class="icons__item">
        <img :src="fruitShop" alt="" class="icons__item__img">
        <p class="icons__item__desc">水果店</p>
      </div>
      <div class="icons__item">
        <img :src="flower" alt="" class="icons__item__img">
        <p class="icons__item__desc">鲜花绿植</p>
      </div>
      <div class="icons__item">
        <img :src="medicine" alt="" class="icons__item__img">
        <p class="icons__item__desc">医药健康</p>
      </div>
      <div class="icons__item">
        <img :src="home" alt="" class="icons__item__img">
        <p class="icons__item__desc">家居时尚</p>
      </div>
      <div class="icons__item">
        <img :src="cake" alt="" class="icons__item__img">
        <p class="icons__item__desc">烘焙蛋糕</p>
      </div>
      <div class="icons__item">
        <img :src="signIn" alt="" class="icons__item__img">
        <p class="icons__item__desc">签到</p>
      </div>
      <div class="icons__item">
        <img :src="big" alt="" class="icons__item__img">
        <p class="icons__item__desc">大牌免运</p>
      </div>
      <div class="icons__item">
        <img :src="redEnvelope" alt="" class="icons__item__img">
        <p class="icons__item__desc">红包套餐</p>
      </div>
    </div>
  <div class="gap"></div>
</template>

<script>
import banner from '@/image/banner.jpg'

import supermarket from '@/image/supermarket.png'
import vegetableMarket from '@/image/vegetable-market.png'
import fruitShop from '@/image/fruit-shop.png'
import flower from '@/image/flower.png'
import medicine from '@/image/medicine.png'
import home from '@/image/home.png'
import cake from '@/image/cake.png'
import signIn from '@/image/sign-in.png'
import big from '@/image/big.png'
import redEnvelope from '@/image/red-envelope.png'

export default {
  name: 'StaticPart',
  props: {
  },
  data () {
    return {
      banner,
      supermarket,
      vegetableMarket,
      fruitShop,
      flower,
      medicine,
      home,
      cake,
      signIn,
      big,
      redEnvelope
    }
  }
}

</script>
<style lang="scss">
@import '@/style/viriables.scss';
@import '@/style/mixins.scss';
.position {
    color: $content-font-color;
    position: relative;
    padding:  .16rem .24rem .16rem 0;
    line-height: .22rem;
    font-size: .16rem;
    @include ellipsis;
    &__icon {
      position: relative;
      top: .02rem;
      font-size: .2rem;
    }
    &__notice {
      position: absolute;
      top: .18rem;
      right: 0;
      font-size: .2rem;
    }
  }
</style>
