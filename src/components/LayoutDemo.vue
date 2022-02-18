<template>
  <div>
    Layout组件
    <h1>示例一</h1>
      <Layout style="height: 20vh;width: 20vw;">
        <Header>头Header</Header>
        <Content>主要Content</Content>
        <Footer>足Footer</Footer>
      </Layout>

    <h1>示例二</h1>
    <Layout style="height: 20vh;width: 20vw;">
      <Header>头Header</Header>
      <Layout class="hasSider">
        <Sider>侧边Sider</Sider>
        <Content>主要Content</Content>
      </Layout>
      <Footer>足Footer</Footer>
    </Layout>

    <h1>示例三</h1>
    <Layout style="height: 20vh;width: 20vw;">
      <Header>头Header</Header>
      <Layout  class="hasSider">
        <Content>主要Content</Content>
        <Sider>侧边Sider</Sider>
      </Layout>
      <Footer>足Footer</Footer>
    </Layout>
    <h1>示例四</h1>
    <Layout class="hasSider" style="height: 20vh;width: 20vw;">
      <Sider>侧边Sider</Sider>
      <Layout>
      <Header>头Header</Header>
      <Content>主要Content</Content>
      <Footer>足Footer</Footer>
      </Layout>
    </Layout>
  </div>
</template>
<script>
import Content from "../lib/Content.vue";
import Layout from "../lib/Layout.vue";
import Header from "../lib/Header.vue";
import Footer from "../lib/Footer.vue";
import Sider from "../lib/Sider.vue";

export default {
  components: {Sider, Footer, Header, Layout, Content}
}
</script>
<style lang="scss" scoped>
* {
  border: blue 1px solid;
}

.demo {
  width: 200px;
  height: 200px;
}
</style>