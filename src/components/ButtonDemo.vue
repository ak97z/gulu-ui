<template>
    <h1>Button组件</h1>
    <Demo :component="Button1Demo"/>
    <Demo :component="Button2Demo"/>
    <Demo :component="Button3Demo"/>
    <Demo :component="Button4Demo"/>
    <Demo :component="Button5Demo"/>
    <Demo :component="Button6Demo"/>
</template>
<script lang="ts">
import Button from '../lib/Button.vue';
import Button1Demo from './Button/Button1.demo.vue';
import Button2Demo from './Button/Button2.demo.vue';
import Button3Demo from './Button/Button3.demo.vue';
import Button4Demo from './Button/Button4.demo.vue';
import Button5Demo from './Button/Button5.demo.vue';
import Button6Demo from './Button/Button6.demo.vue';
import Demo from './Demo.vue';


export default {
  components: {Button,Demo},

  setup() {
    return {
      Button1Demo,Button2Demo,Button3Demo,Button4Demo,Button5Demo,Button6Demo,
    };
  }
};
</script>
