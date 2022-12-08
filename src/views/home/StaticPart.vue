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
      <div class="icons__item" v-for="(item, index) in iconsList" :key="index">
        <img :src="item.imageUrl" alt="" class="icons__item__img">
        <p class="icons__item__desc">{{item.desc}}</p>
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
  setup () {
    const iconsList = [
      {
        imageUrl: supermarket,
        desc: '超市便利'
      },
      {
        imageUrl: vegetableMarket,
        desc: '菜市场'
      },
      {
        imageUrl: fruitShop,
        desc: '水果店'
      },
      {
        imageUrl: flower,
        desc: '鲜花绿植'
      },
      {
        imageUrl: medicine,
        desc: '医药健康'
      },
      {
        imageUrl: home,
        desc: '家居时尚'
      },
      {
        imageUrl: cake,
        desc: '烘焙蛋糕'
      },
      {
        imageUrl: signIn,
        desc: '签到'
      },
      {
        imageUrl: big,
        desc: '大牌免运'
      },
      {
        imageUrl: redEnvelope,
        desc: '红包套餐'
      }
    ]
    return {
      banner,
      iconsList
    }
  }
}

</script>
<style lang="scss" scoped>
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
</style>
