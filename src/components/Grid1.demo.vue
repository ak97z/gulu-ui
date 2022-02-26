<demo>
基础用法
</demo>
<template>
  <Row>
    <Col span="1">
      <Col>4</Col>
    </Col>
    <Col span="3">2</Col>
    <Col span="20">3</Col>
  </Row>
</template>
<script>
import Row from "../lib/Row.vue";
import Col from "../lib/Col.vue";

export default {components: {Row, Col}}
</script>