<demo>
内容方位
</demo>

<template>
  <Popover content="内容在上方" position="top"  trigger="hover">
    <Button>内容在上方</Button>
  </Popover>
  <Popover content="内容在下方" position="bottom"  trigger="hover">
    <Button>内容在下方</Button>
  </Popover>


</template>
<script>
import Popover from "../../lib/Popover.vue";
import Button from "../../lib/Button.vue";

export default {
  components: {Button, Popover,}
}
</script>