<demo>
基础用法
</demo>
<template>
  <Row>
    <Col span="3"  style="background: #999999">3</Col>
    <Col span="1" style="background: #add8e6">1</Col>
    <Col span="20" style="background: #e1e4e8">20</Col>
  </Row>
</template>
<script>
import Row from "../../lib/Row.vue";
import Col from "../../lib/Col.vue";

export default {components: {Row, Col}}
</script>