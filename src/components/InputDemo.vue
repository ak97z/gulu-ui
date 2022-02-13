<template>
  <h1>Input示例1</h1>
  <Input value="第一天,错误信息" error="输入不合法,请重新输入"/>
  <Input value="第二天,不可选" disabled/>
  <Input value="第三天,只读" readonly/>

</template>
<script>
import Input from "../lib/Input.vue";
export default {
  components: {Input}
}
</script>