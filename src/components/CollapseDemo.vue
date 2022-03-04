<template>
  <h1>Collapse组件</h1>
  <Demo :component="Collapse1Demo"/>

</template>

<script lang="ts">
import Demo from './Demo.vue';
import Collapse1Demo from './Collapse/Collapse1.demo.vue';

export default {
  components: {Demo},
  setup() {return {Collapse1Demo};}
};
</script>