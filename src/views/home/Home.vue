<template>
  <div class="wrapper">
  <StaticPart />
  <HomeNearby />
  </div>
  <HomeDocker />
</template>
<script>
import StaticPart from '@/views/home/StaticPart'
import HomeNearby from './Nearby'
import HomeDocker from './Docker'
export default {
  name: 'HomeHome',
  data () {
    return {}
  },
  components: {
    StaticPart,
    HomeNearby,
    HomeDocker
  }
}
</script>
<style lang="scss">
@import '@/style/viriables.scss';
@import '@/style/mixins.scss';
.wrapper {
  overflow-y: auto;
  position: absolute;
  left: 0;
  bottom: 0.5rem;
  top: 0;
  right: 0;
  padding: 0 .18rem .1rem .18rem;
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
