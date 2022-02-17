<template>
  <div class="row" :style="{marginLeft: -gutter/2+'px', marginRight: -gutter/2+'px'}">
    <slot></slot>
  </div>
</template>
<script>
import Col from "./Col.vue";
import {provide, ref} from "vue";

export default {
components:{
  Col
},
  setup(){
    function gutter() {
      let gutter = props.gutter

    }

    const gut=ref(gutter)
      provide('xxx',gut)
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
    console.log(this)
    console.log(this.$children)
    // this.$children.forEach((vm) => {
    //   vm.gutter = this.gutter
    // })
  }
}

</script>
<style lang="scss" scoped>
.row {
  border: green 1px solid;
  display: flex;
}
</style>
