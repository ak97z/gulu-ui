<template>
  <h1>Input示例1</h1>
  <Input value="第一天" error="输入不合法,请重新输入"/>
  <Input value="第二天" disabled/>
  <Input value="第三天" readonly/>

</template>
<script>
import Input from "../lib/Input.vue";
export default {
  components: {Input}
}
</script>