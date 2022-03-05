<demo>
基础用法
</demo>
<template>
  <Collapse>
    <CollapseItem title="title1">content1</CollapseItem>
    <CollapseItem title="title2">content2</CollapseItem>
    <CollapseItem title="title3">content3</CollapseItem>
  </Collapse>
</template>
<script>

import Collapse from "../../lib/Collapse.vue";
import CollapseItem from "../../lib/Collapse-Item.vue";

export default {
  components: {Collapse,CollapseItem}
}
</script>
