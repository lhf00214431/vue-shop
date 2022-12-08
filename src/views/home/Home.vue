<template>
  <div class="wrapper">
  <StaticPart />
  <HomeNearby />
  </div>
  <HomeDocker />
</template>
<script>
import StaticPart from '@/views/home/StaticPart'
import HomeNearby from '@/views/home/Nearby'
import HomeDocker from '@/views/home/Docker'
export default {
  name: 'HomeHome',
  components: {
    StaticPart,
    HomeNearby,
    HomeDocker
  }
}
</script>
<style lang="scss" scoped>
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
}
</style>
