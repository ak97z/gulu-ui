<template>
  <h1>Dialog组件</h1>
  <Demo :component="Tab1Demo"/>

</template>

<script lang="ts">
import Demo from './Demo.vue';
import Tab1Demo from './Tab/Tab1.demo.vue';

export default {
  components: {Demo},
  setup() {return {Tab1Demo};}
};
</script>