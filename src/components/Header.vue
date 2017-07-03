<template lang="pug">
div
  OverlayNav(ref="search")
  div.nav(v-bind:class="{responsive:counter%2==1}")
    a.home(href="#")
      i.fa.fa-chevron-left 
      span  Home
    i.fa.fa-fw.fa-bars.menu(@click="open('openMenu')")
    i.fa.fa-fw.fa-search.search(@click="open('openSearch')")
</template>

<script>
import OverlayNav from '@/components/Navigation/OverlayNav';

export default {
  components: {
    OverlayNav,
  },
  methods: {
    open(action) {
      this.$refs.search.action = action;
    },
  },
  data() {
    return {
      searchStatus: 'opened',
      isHovered: 'false',
      counter: 0,
    };
  },
};
</script>

<style lang="stylus" scoped>
.nav 
  overflow hidden
  a.home
    color #000
    border 0.3125rem solid #000
    padding 0.625rem 1.5625rem 0.5625rem
    text-align center
    text-decoration none
    font-size 1.0625rem
    font-weight 700
    text-transform uppercase
    margin-left 1.875rem
    margin-top 1.5625rem
    float left
    font-family 'Source Sans Pro', sans-serif
    i.fa
      font-size 0.875em
      transition all .3s
    &:hover i.fa
      transform translateX(-0.3125rem)

  i.fa.fa-fw
    cursor pointer
    margin-top 1.875rem
    font-size 2.5rem
    float right
    &.menu
      margin-right 1.875rem
    &.search
      margin-right .625rem
</style>

