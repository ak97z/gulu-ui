<template>
  <div>Dialog示例</div>
  <Button @click="toggle">toggle</Button>
  <Dialog v-model:visible="x" :closeOnClickOverlay="false" :ok="f1" :cancel="f2">
   <div>自定义内容</div>
  </Dialog>
  <!--   <Dialog :visible="x" @update:visible="x = $event"/>-->

</template>

<script lang="ts">
import Dialog from '../lib/Dialog.vue';
import Button from '../lib/Button.vue';
import {ref} from 'vue';

export default {
  components: {Dialog, Button},
  setup() {
    const x = ref(false);
    const toggle = () => {
      x.value = !x.value;
    };
    const f1 = () => {
      return true
    };
    const f2 = () => {
      return false
    };
    return {x, toggle, f1, f2};
  }
};
</script>