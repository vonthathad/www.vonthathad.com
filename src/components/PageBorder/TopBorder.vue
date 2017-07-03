<template lang="pug">
div.tborder
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
.tborder
    position fixed
    top 0
    left 0
    right 0
    height .9375rem
    background-color #000
</style>

