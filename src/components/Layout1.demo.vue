<demo>
基础用法
</demo>
<template>
  <Layout style="height: 50vh;width: 50vw;">
    <Header>头Header</Header>
    <Content>主要Content</Content>
    <Footer>足Footer</Footer>
  </Layout>
</template>
<script>
import Content from "../lib/Content.vue";
import Layout from "../lib/Layout.vue";
import Header from "../lib/Header.vue";
import Footer from "../lib/Footer.vue";

export default {components: {Layout, Header, Content, Footer}}
</script>