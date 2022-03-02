<demo>
默认用法
</demo>

<template >
  <Popover content="1popover内容2popover内容3popover内容4popover内容5popover内容6popover内容">
    <Button>默认按钮</Button>
  </Popover>
</template>
<script>
import Popover from "../../lib/Popover.vue";
import Button from "../../lib/Button.vue";

export default {
  components: {Button, Popover,}
}
</script>