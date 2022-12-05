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
      <img src="" alt="">
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

<style lang="scss">
@import './style/viriables.scss';
@import './style/mixins.scss';
.wrapper {
  position: absolute;
  left: 0;
  bottom: 0.5rem;
  top: 0;
  right: 0;
  padding: 0 .18rem;
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
.docker {
  display: flex;
  box-sizing: border-box;
  position:absolute;
  padding: 0 .18rem;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 0.49rem;
  border-top: 0.01rem solid #F1F1F1;
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
