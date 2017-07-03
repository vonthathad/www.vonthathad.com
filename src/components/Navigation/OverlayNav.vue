<template lang="pug">
  div.container(v-bind:class="{open:action!='close'}")
    i.fa.fa-times.close(@click="onClose")
    Search(v-if="action=='openSearch'")
    Menu_(v-if="action=='openMenu'")
</template>

<script>
import Search from '@/components/Navigation/Search';
import Menu_ from '@/components/Navigation/Menu';

export default {
  components: {
    Search,
    Menu_,
  },
  data() {
    return {
      action: 'close',
    };
  },
  methods: {
    onClose() {
      this.action = 'close';
    },
  },
};
</script>

<style lang="stylus" scoped>
.container
  &.open 
    visibility visible
    opacity 1
    transition opacity .5s
  position fixed
  background rgba(0,0,0,.95)
  width 100%
  min-height 100%
  visibility hidden
  opacity 0
  top 0
  left 0
  overflow-y auto
  z-index 1
  .close
    color #fff
    font-size 3.75rem
    position absolute
    right 3.0875rem
    top 2.1875rem
    cursor pointer
</style>

