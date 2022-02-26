<template>
  <h1>Input示例1</h1>
  <Demo :component="Input1Demo"/>
  <Demo :component="Input2Demo"/>
  <Demo :component="Input3Demo"/>


</template>
<script>
import Input1Demo from './Input1.demo.vue';
import Input2Demo from './Input2.demo.vue';
import Input3Demo from './Input3.demo.vue';
import Demo from './Demo.vue';

export default {
  components: {Demo},
  setup() {return {Input1Demo, Input2Demo,Input3Demo}}
}
</script>