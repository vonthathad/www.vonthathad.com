<template lang="pug">
div.rborder
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
.rborder
    position fixed
    bottom 0
    right 0
    top 0
    width .9375rem
    background-color #000
</style>

