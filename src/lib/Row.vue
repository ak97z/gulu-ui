<template>
  <div class="row" :style="rowStyle" :class="rowClass">
    <slot></slot>
  </div>
</template>
<script>
import Col from "./Col.vue";

export default {
components:{Col},
  computed: {
    rowStyle () {
      let {gutter} = this
      return {marginLeft: -gutter / 2 + 'px', marginRight: -gutter / 2 + 'px'}
    },
    rowClass () {
      let {align} = this
      return [align && `align-${align}`]
    }
  },


  props: {
    gutter: {
      type: [Number, String]
    }
  },
}

</script>
<style scoped lang="scss">
.row{
  display: flex;
  flex-wrap: wrap;
  &.align-left {
    justify-content: flex-start;
  }
  &.align-right {
    justify-content: flex-end;
  }
  &.align-center {
    justify-content: center;
  }
}
</style>
