<demo>
基础用法(点击Overlay区域可退出)
</demo>
<template>
  <Button @click="showDialog">show</Button>
</template>
<script>

import Button from "../../lib/Button.vue";
import Dialog from "../../lib/Dialog.vue";
import {openDialog} from "../../lib/openDialog";

export default {
  components: {Button, Dialog},
  setup() {
    const showDialog = () => {
      openDialog({title: '自定义标题', content: '自定义内容', ok() {}, cancel() {}})}
    return {showDialog}
  }
}
</script>