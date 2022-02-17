<template>
  <div class="col" :class="[span && `col-span-${span}`,gutter && `col-gutter-${gutter}`]"
       :style="{paddingLeft: gutter/2+'px', paddingRight: gutter/2+'px'}"
  >
    <div style="border: 1px solid green; height: 100px;">
      <slot></slot>
    </div>

  </div>
</template>
<script>


export default {

  // computed: {
  //   gutter() {
  //     let parent = this.$parent;
  //     console.log(parent.gutter);
  //     while (parent && parent.$options.componentName !== 'Row') {
  //       parent = parent.$parent;
  //     }
  //     return parent ? parent.gutter : 0;
  //
  //   },
  // },

  props: {
    // gutter: {
    // default:parent.gutter
    // },
    span: {
      type: [String, Number]
    }
  },
  data() {
    // console.log("render"+this.$parent.gutter);
    // let parent = this.$parent;
    // return {gutter: this.$parent.gutter}
    return {gutter: this.$parent.gutter}
  },
  // render(h) {
  //   console.log("render"+parent.gutter);
  //   if (parent.gutter) {
  //     style.paddingLeft = this.gutter / 2 + 'px';
  //     style.paddingRight = style.paddingLeft;
  //   }
  // },
}
</script>
<style lang="scss" scoped>
.col {

  width: 50%;
  height: 100px;
  $class-prefix: col-span-;
  @for $n from 1 through 24 {
    &.#{$class-prefix}#{$n} {
      width: ($n/24)*100%;
    }
  }
}
</style>