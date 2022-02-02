<template>
  <div>
    Tabs组件
    <component :is="defaults[0]"/>
    <component :is="defaults[1]"/>
  </div>
</template>
<script lang="ts">
import Tab from '../lib/Tab.vue';
export default {
  setup(props, context) {
    console.log(context.slots.default());
    const defaults = context.slots.default();
    defaults.forEach((tag) => {
      if (tag.type !== Tab) {
        throw new Error('Tabs组件的子组件必须是Tab');
      }
    });
    return {
      defaults
    };
  }
};

</script>