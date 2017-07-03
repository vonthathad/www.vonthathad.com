
<template lang="pug">
  div.wrapper
    Navbar
    router-view
    TopBorder
    BottomBorder
    LeftBorder
    RightBorder
</template>

<script>
import Navbar from '@/components/Header';
import TopBorder from '@/components/PageBorder/TopBorder';
import BottomBorder from '@/components/PageBorder/BottomBorder';
import LeftBorder from '@/components/PageBorder/LeftBorder';
import RightBorder from '@/components/PageBorder/RightBorder';

export default {
  components: {
    Navbar,
    TopBorder,
    BottomBorder,
    LeftBorder,
    RightBorder,
  },
  name: 'app',
};
</script>

<style lang='stylus'>
body
  margin 0
  padding 0.9375rem
</style>
