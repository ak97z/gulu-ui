<demo>
自定义用法(带Input组件,点击Overlay区域不可退出)
</demo>
<template>
  <Button @click="toggle">toggle</Button>
  <Dialog v-model:visible="x"
          :ok="ok"
          :cancel="cancel"
          :closeOnClickOverlay="false">
    <template v-slot:content>
      <div>自定义内容  <Input value="自定义内容" error="自定义error"/></div>
    </template>
    <template v-slot:title>
      <strong>自定义标题</strong>
    </template>
  </Dialog>
</template>

<script>
import Dialog from "../../lib/Dialog.vue";
import {ref} from "vue";
import Button from "../../lib/Button.vue";
import Input from "../../lib/Input.vue";
export default {
  components: {Dialog,Button,Input},
  setup() {
    const x = ref(false);
    const toggle = () => {x.value = !x.value;};
    const ok = () => {return {}};
    const cancel = () => {return {}};
    return {x, toggle, ok, cancel}}
}
</script>