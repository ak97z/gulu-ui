<demo>
侧边栏(左)
</demo>
<template>
  <Layout style="height: 50vh;width: 50vw;">
    <Header>头Header</Header>
    <Layout class="hasSider">
      <Sider>侧边Sider</Sider>
      <Content>主要Content</Content>
    </Layout>
    <Footer>足Footer</Footer>
  </Layout>
</template>
<script>
import Content from "../../lib/Content.vue";
import Layout from "../../lib/Layout.vue";
import Header from "../../lib/Header.vue";
import Footer from "../../lib/Footer.vue";
import Sider from "../../lib/Sider.vue";

export default {components: {Layout,Header,Content,Footer,Sider}}
</script>