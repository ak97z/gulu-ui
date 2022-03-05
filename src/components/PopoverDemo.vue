<template>
  <h1>Popover组件</h1>
  <Demo :component="Popover1Demo"/>
  <Demo :component="Popover2Demo"/>

</template>

<script lang="ts">
import Demo from './Demo.vue';
import Popover1Demo from './Popover/Popover1.demo.vue';
import Popover2Demo from './Popover/Popover2.demo.vue';
export default {
  components: {Demo},
  setup() {return {Popover1Demo,Popover2Demo};}
};
</script>