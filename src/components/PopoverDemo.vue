<template>
  <h1>Popover组件</h1>
  <Demo :component="Popover1Demo"/>

</template>

<script lang="ts">
import Demo from './Demo.vue';
import Popover1Demo from './Popover/Popover1.demo.vue';

export default {
  components: {Demo},
  setup() {return {Popover1Demo};}
};
</script>