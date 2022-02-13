<template>
  <div class="col" :class="[span && `col-${span}`]" :style="{paddingLeft: gutter/2+'px', paddingRight: gutter/2+'px'}">
    <div style="border: 1px solid green; height: 100px;">
      <slot></slot>
    </div>

  </div>
</template>
<script>
export default {
  props: {

    span: {
      type: [String, Number]
    }
  },
  data() {
    return {gutter: 0}
  },

}
</script>
<style lang="scss" scoped>
.col {

  width: 50%;
  height: 100px;
  $class-prefix: col-;
  @for $n from 1 through 24 {
    &.#{$class-prefix}#{$n} {
      width: ($n/24)*100%;
    }
  }
}
</style>