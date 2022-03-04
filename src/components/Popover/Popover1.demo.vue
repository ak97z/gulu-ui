<demo>
手动激活
</demo>

<template>
  <Popover content="1popover内容"
           position="top">
    <Button>click(上)</Button>
  </Popover>
  <Popover content="1popover内容"
           position="bottom"
  trigger="hover">
    <Button>hover(下)</Button>
  </Popover>


</template>
<script>
import Popover from "../../lib/Popover.vue";
import Button from "../../lib/Button.vue";

export default {
  components: {Button, Popover,}
}
</script>