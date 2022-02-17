<template>
  <h1>Row示例</h1>
  <Row gutter="10">
    <Col span="1">1</Col>
    <Col span="3">2</Col>
    <Col span="20">3</Col>
  </Row>
  <Row gutter="20">
    <Col span="20">11</Col>
    <Col span="3">22</Col>
    <Col span="1">33</Col>
  </Row>
</template>
<script>
import Row from "../lib/Row.vue";
import Col from "../lib/Col.vue";

export default {
  components:{
    Row,Col,
  }
}
</script>