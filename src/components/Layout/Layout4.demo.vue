<demo>
侧边栏(整体)
</demo>
<template>
  <Layout class="hasSider" style="height: 50vh;width: 50vw;">
    <Sider>侧边Sider</Sider>
    <Layout>
      <Header>头Header</Header>
      <Content>主要Content</Content>
      <Footer>足Footer</Footer>
    </Layout>
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