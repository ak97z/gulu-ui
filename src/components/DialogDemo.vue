<template>
  <div>Dialog示例1</div>
  <h1>示例1</h1>
  <Button @click="toggle">toggle</Button>
  <Dialog v-model:visible="x" :closeOnClickOverlay="false" :ok="f1" :cancel="f2">
    <template v-slot:content>
      <div>自定义内容</div>
    </template>
    <template v-slot:title>
      <strong>自定义标题</strong>
    </template>
  </Dialog>
  <!--   <Dialog :visible="x" @update:visible="x = $event"/>-->
<h1>示例2</h1>
  <Button @click="showDialog">show</Button>

</template>

<script lang="ts">
import Dialog from '../lib/Dialog.vue';
import Button from '../lib/Button.vue';
import {ref} from 'vue';
import {openDialog} from '../lib/openDialog';

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
    const showDialog = ()=>{
      openDialog({
        title:'标题一句话',
        content:'内容 一句话',
        ok(){
          console.log('ok');
        },
        cancel(){
          console.log('cancel');
        }
      })
    }
    return {x, toggle, f1, f2,showDialog};
  }
};
</script>