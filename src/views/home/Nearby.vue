<template>
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
</template>

<script>
import near from '@/image/near.png'
export default {
  name: 'HomeNearby',
  props: {
  },
  data () {
    return {
      near
    }
  }
}

</script>
<style scoped>
</style>
