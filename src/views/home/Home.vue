<template>
  <div class="wrapper">
  <StaticPart />
  <Nearby />
  </div>
  <Docker />
</template>
<script>
import StaticPart from '@/views/home/StaticPart'
import Nearby from '@/views/home/Nearby'
import Docker from '@/views/home/Docker'
export default {
  name: 'Home',
  components: {
    StaticPart,
    Nearby,
    Docker
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
