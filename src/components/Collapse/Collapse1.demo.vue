<demo>
基础用法
</demo>
<template>
  <Collapse>
    <CollapseItem title="title1">1content</CollapseItem>
    <CollapseItem title="title2">2content</CollapseItem>
    <CollapseItem title="title3">3content</CollapseItem>
  </Collapse>
</template>
<script>

import Collapse from "../../lib/Collapse.vue";
import CollapseItem from "../../lib/Collapse-Item.vue";

export default {
  components: {Collapse,CollapseItem}
}
</script>
