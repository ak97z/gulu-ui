<demo>
支持gutter参数
</demo>
<template>
  <Row gutter="20">
    <Col span="20">11</Col>
    <Col span="3">22</Col>
    <Col span="1">33</Col>
  </Row>
</template>
<script>
import Row from "../lib/Row.vue";
import Col from "../lib/Col.vue";

export default {components: {Row, Col}}
</script>