<demo>
支持gutter参数
</demo>
<template>
  <Row gutter="20">
    <Col>gutter为20</Col>
    <Col>gutter为20</Col>
    <Col>gutter为20</Col>
  </Row>
</template>
<script>
import Row from "../../lib/Row.vue";
import Col from "../../lib/Col.vue";

export default {components: {Row, Col}}
</script>