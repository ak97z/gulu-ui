<demo>
激活方式
</demo>

<template>

  <Popover content="悬停激活" trigger="hover">
    <Button>hover</Button>
  </Popover>
  <Popover content="点击激活">
    <Button>click</Button>
  </Popover>

</template>
<script>
import Popover from "../../lib/Popover.vue";
import Button from "../../lib/Button.vue";

export default {
  components: {Button, Popover,}
}
</script>