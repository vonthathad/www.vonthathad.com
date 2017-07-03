<template lang="pug">
div.search-container
  div.row
    form
      input.search-input(placeholder="Search...")
  div.row
    div.results
      p Number of posts found: 13
      a(href="") 
        h2
          i.fa.fa-fw.fa-dot-circle-o
          span  Meteor Accounts based on sId package
      a(href="") 
        h2
          i.fa.fa-fw.fa-dot-circle-o
          span  Meteor Accounts based on sId package
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
.search-container
  margin-top 11%
  padding-left 1.25rem
  padding-right 1.25rem
  .row
    max-width 50rem
    padding-left .9375rem
    padding-right .9375rem
    margin 0 auto
    .search-input
      background-color transparent
      height 4.5rem
      font-size 3.125rem
      color #ffffff
      border 0
      border-bottom .1875rem solid #fff
      padding 1.25rem 0
      font-family 'Source Sans Pro',sans-serif
      font-weight 900
      width 100%
      &::placeholder
        color #fff
      &:focus
        outline none
    .results
      color #fff
      font-family 'Source Sans Pro',sans-serif
      p
        font-weight 600
        font-size 2.25rem
        padding-bottom .9375rem
        padding-top .9375rem
      a
        text-decoration none
        color #fff
        h2
          font-size 1.75rem
          font-weight 400
</style>

