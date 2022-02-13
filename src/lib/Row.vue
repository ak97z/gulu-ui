<template>
  <div class="row" :style="{marginLeft: -gutter/2+'px', marginRight: -gutter/2+'px'}">
    <slot></slot>
  </div>
</template>
<script>
import Col from "./Col.vue";
export default {
components:{
  Col
},
  props: {
    gutter: {
      type: [Number, String]
    }
  },
  created () {
    console.log('row created')
  },
  mounted () {
    console.log('row mounted')
    console.log(this.$children)
    this.$children.forEach((vm) => {
      vm.gutter = this.gutter
    })
  }
}

</script>
<style lang="scss" scoped>
.row {
  border: green 1px solid;
  display: flex;
}
</style>
