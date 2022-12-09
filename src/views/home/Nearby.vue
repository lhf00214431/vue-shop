<template>
  <div class="nearby">
    <h3 class="nearby__title">附近店铺</h3>
    <div class="nearby__item" v-for="(item, index) in nearbyList" :key="index">
      <img :src="item.imgUrl" alt="" class="nearby__item__img">
      <div class="nearby__item__content">
        <div class="nearby__item__content__title">{{item.title}}</div>
        <div class="nearby__item__content__tags">
          <span class="nearby__item__content__tags__tag" v-for="(innerItem, innerIndex) in item.tags" :key="'inner' + innerIndex">{{innerItem}}</span>
        </div>
        <p class="nearby__item__content__highlight">{{item.highlight}}(每月3张)</p>
      </div>
    </div>
  </div>
</template>

<script scoped>
import near from '@/image/near.png'
export default {
  name: 'Nearby',
  props: {
  },
  setup () {
    const nearbyList = [
      {
        title: '沃尔玛',
        imgUrl: near,
        tags: ['月售1万+', '起送￥0', '基础运费￥5'],
        highlight: 'VIP尊享满89元减4元运费'
      },
      {
        title: '沃尔玛',
        imgUrl: near,
        tags: ['月售1万+', '起送￥0', '基础运费￥5'],
        highlight: 'VIP尊享满89元减4元运费'
      },
      {
        title: '沃尔玛',
        imgUrl: near,
        tags: ['月售1万+', '起送￥0', '基础运费￥5'],
        highlight: 'VIP尊享满89元减4元运费'
      },
      {
        title: '沃尔玛',
        imgUrl: near,
        tags: ['月售1万+', '起送￥0', '基础运费￥5'],
        highlight: 'VIP尊享满89元减4元运费'
      },
      {
        title: '沃尔玛',
        imgUrl: near,
        tags: ['月售1万+', '起送￥0', '基础运费￥5'],
        highlight: 'VIP尊享满89元减4元运费'
      }
    ]
    return {
      nearbyList
    }
  }
}

</script>
<style lang="scss" scoped>
@import '@/style/viriables.scss';
@import '@/style/mixins.scss';

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
</style>
