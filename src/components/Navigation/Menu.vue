<template lang="pug">
div.nav2
  ul
    li
      a(href="#") Home
    li
      a(href="#") About
    li
      a(href="#") Projects
    li 
      a(href="#")
        i.fa.fa-fw.fa-envelope
      a(href="#")
        i.fa.fa-fw.fa-github
      a(href="#")
        i.fa.fa-fw.fa-facebook
    
</template>

<script>
export default {
  data() {
    return {
      action: 'closed',
    };
  },
  methods: {
    onClose() {
      this.action = 'closed';
    },
  },
};
</script>

<style lang="stylus" scoped>
.nav2
  text-align center
  height 400px
  top 50%
  transform translateY(50%)
  ul
    display block
    list-style none
    padding 0 
    margin 0 auto
    height 100%
    li
      display block
      height (100% / 4)
      a
        font-weight 300
        font-size 3.375rem
        text-decoration none
        color #fff
        font-family 'Source Sans Pro',sans-serif
        &:hover
          color #808080
</style>

