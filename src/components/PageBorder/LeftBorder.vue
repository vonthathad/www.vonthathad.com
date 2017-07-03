<template lang="pug">
div.lborder
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
.lborder
    position fixed
    bottom 0
    left 0
    top 0
    width .9375rem
    background-color #000
</style>

