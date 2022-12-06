<template>
  <div class="wrapper">
    <div class="position">
      <span class="iconfont position__icon">&#xe67f;</span>
      地址地址地支地址地址地址地支地址地址地址地支地址地址地址地支地址
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
  <div class="nearby">
    <h3 class="nearby__title">附近店铺</h3>
    <div class="nearby__item">
      <img :src="near" alt="" class="nearby__item__img">
      <div class="nearby__item__content">
        <div class="nearby__item__content__title">沃尔玛</div>
        <div class="nearby__item__content__tags">
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
        </div>
        <p class="nearby__item__content__highlight">VIP尊享满89元减4元运费(每月3张)</p>
      </div>
    </div>
    <div class="nearby__item">
      <img :src="near" alt="" class="nearby__item__img">
      <div class="nearby__item__content">
        <div class="nearby__item__content__title">沃尔玛</div>
        <div class="nearby__item__content__tags">
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
        </div>
        <p class="nearby__item__content__highlight">VIP尊享满89元减4元运费(每月3张)</p>
      </div>
    </div>
    <div class="nearby__item">
      <img :src="near" alt="" class="nearby__item__img">
      <div class="nearby__item__content">
        <div class="nearby__item__content__title">沃尔玛</div>
        <div class="nearby__item__content__tags">
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
        </div>
        <p class="nearby__item__content__highlight">VIP尊享满89元减4元运费(每月3张)</p>
      </div>
    </div>
    <div class="nearby__item">
      <img :src="near" alt="" class="nearby__item__img">
      <div class="nearby__item__content">
        <div class="nearby__item__content__title">沃尔玛</div>
        <div class="nearby__item__content__tags">
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
        </div>
        <p class="nearby__item__content__highlight">VIP尊享满89元减4元运费(每月3张)</p>
      </div>
    </div>
    <div class="nearby__item">
      <img :src="near" alt="" class="nearby__item__img">
      <div class="nearby__item__content">
        <div class="nearby__item__content__title">沃尔玛</div>
        <div class="nearby__item__content__tags">
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
        </div>
        <p class="nearby__item__content__highlight">VIP尊享满89元减4元运费(每月3张)</p>
      </div>
    </div>
    <div class="nearby__item">
      <img :src="near" alt="" class="nearby__item__img">
      <div class="nearby__item__content">
        <div class="nearby__item__content__title">沃尔玛</div>
        <div class="nearby__item__content__tags">
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
          <span class="nearby__item__content__tags__tag">月售1万+</span>
        </div>
        <p class="nearby__item__content__highlight">VIP尊享满89元减4元运费(每月3张)</p>
      </div>
    </div>
  </div>
  </div>
  <div class="docker">
    <div class="docker__item docker__item--active">
      <div class="iconfont">&#xe7a7;</div>
      <div class="cocker__title">首页</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe6af;</div>
      <div class="cocker__title">购物车</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe60e;</div>
      <div class="cocker__title">订单</div>
    </div>
    <div class="docker__item">
      <div class="iconfont">&#xe78b;</div>
      <div class="cocker__title">我的</div>
    </div>
  </div>
</template>
<script>
import banner from './image/banner.jpg'

import supermarket from './image/supermarket.png'
import vegetableMarket from './image/vegetable-market.png'
import fruitShop from './image/fruit-shop.png'
import flower from './image/flower.png'
import medicine from './image/medicine.png'
import home from './image/home.png'
import cake from './image/cake.png'
import signIn from './image/sign-in.png'
import big from './image/big.png'
import redEnvelope from './image/red-envelope.png'

import near from './image/near.png'
export default {
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
      redEnvelope,
      near
    }
  }
}
</script>
<style lang="scss">
@import './style/viriables.scss';
@import './style/mixins.scss';
.wrapper {
  overflow-y: auto;
  position: absolute;
  left: 0;
  bottom: 0.5rem;
  top: 0;
  right: 0;
  padding: 0 .18rem .1rem .18rem;
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
  .search {
    line-height: .32rem;
    background: #F5F5F5;
    color:#B7B7B7;
    border-radius: .16rem;
    font-size: .14rem;
    &__icon {
      position: relative;
      top: .02rem;
      display: inline-block;
      font-size: .2rem;
      padding: 0 .06rem 0 .16rem;
    }
  }
}
.banner {
  height: 0;
  overflow: hidden;
  padding-bottom: 25.4%;
  margin-top:.16rem;
  &__image {
    width: 100%
  }
}
.icons {
  display: flex;
  flex-wrap: wrap;
  margin-top:.16rem;
  &__item {
    width:20%;
    &__img {
      display: block;
      width: .4rem;
      height: .4rem;
      margin: 0 auto;
    }
    &__desc {
      margin: 0.06rem 0 .16rem 0;
      text-align:center;
      color: $content-font-color;
    }
  }
}
.gap {
  height: .1rem;
  background-color: $content-bg-color;
  margin: 0 -.18rem;
}
.nearby {
  &__title{
    margin: .16rem 0 .02rem 0;
    font-size: .18rem;
    font-weight: normal;
    color: $content-font-color;
  }
  &__item {
    display: flex;
    padding-top: .12rem;
    &__img{
      margin-right: .16rem;
      width: .56rem;
      height: .56rem;
    }
    &__content{
      flex: 1;
      padding-bottom: .12rem;
      border-bottom: 1px solid $content-bg-color;
      &__title{
        line-height: .2rem;
        font-size: .16rem;
        color: $content-font-color;
      }
      &__tags{
        margin-top: .08rem;
        line-height: .18rem;
        font-size: .13rem;
        color: $content-font-color;
        &__tag{
          margin-right: .16rem;
        }
      }
      &__highlight{
        color:#E93B3B;
        margin: .08rem 0 0 0;
        line-height: .18rem;
        font-size: .13rem;
      }
    }
  }
}
.docker {
  display: flex;
  box-sizing: border-box;
  position:absolute;
  padding: 0 .18rem;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 0.49rem;
  border-top: 0.01rem solid $content-bg-color;
  color: $content-font-color;
  &__item {
    flex: 1;
    text-align: center;
    .iconfont{
      margin: 0.07rem 0 0.02rem 0;
      font-size: .18rem;
    }
    &--active {
      color: #1FA4FC;
    }
  }
  &__title {
    font-size: .2rem;
    transform: scale(0.5 0.5);
    transform-origin: center top;
  }
}
</style>
