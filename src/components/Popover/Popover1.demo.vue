<demo>
手动激活
</demo>

<template>
  <Popover content="1popover内容"
           position="top">
    <Button>手动激活(上)</Button>
  </Popover>
  <Popover content="1popover内容"
           position="bottom">
    <Button>手动激活(下)</Button>
  </Popover>

</template>
<script>
import Popover from "../../lib/Popover.vue";
import Button from "../../lib/Button.vue";

export default {
  components: {Button, Popover,}
}
</script>