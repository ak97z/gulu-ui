<template>
  <h1>Layout组件</h1>
  <Demo :component="Layout1Demo"/>
  <Demo :component="Layout2Demo"/>
  <Demo :component="Layout3Demo"/>
  <Demo :component="Layout4Demo"/>
</template>
<script>
import Demo from './Demo.vue';
import Layout1Demo from './Layout1.demo.vue';
import Layout2Demo from './Layout2.demo.vue';
import Layout3Demo from './Layout3.demo.vue';
import Layout4Demo from './Layout4.demo.vue';


export default {
  components: {Demo},
  setup() {return {Layout1Demo, Layout2Demo, Layout3Demo, Layout4Demo,}}
}
</script>
