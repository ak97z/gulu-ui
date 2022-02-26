<template>
  <h1>Row示例</h1>
  <Demo :component="Grid1Demo"/>
  <Demo :component="Grid2Demo"/>
</template>
<script>
import Grid1Demo from './Grid1.demo.vue';
import Grid2Demo from './Grid2.demo.vue';
import Demo from './Demo.vue';

export default {
  components: {Demo,},
  setup() {return {Grid1Demo, Grid2Demo}}
}
</script>