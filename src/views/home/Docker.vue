<template>
  <div class="docker">
    <div
    v-for="(item, index) in dockerList"
    :key="index"
    :class="{ 'docker__item': true, 'docker__item--active': index === 0 }">
      <div class="iconfont" v-html="item.icon"></div>
      <div class="cocker__title">{{item.text}}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeDocker',
  props: {
  },
  setup () {
    const dockerList = [
      { icon: '&#xe7a7;', text: '首页' },
      { icon: '&#xe6af;', text: '购物车' },
      { icon: '&#xe60e;', text: '订单' },
      { icon: '&#xe78b;', text: '我的' }
    ]
    return { dockerList }
  }
}

</script>
<style lang="scss" scoped>
@import '@/style/viriables.scss';
@import '@/style/mixins.scss';
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
