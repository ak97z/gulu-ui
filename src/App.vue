<template>
  <div>
    导航栏
    <router-link to="/">Frank1</router-link>
    <router-link to="/2">Frank2</router-link>
  </div>
  <router-view/>
</template>


<script>
// import Frank from "./components/Frank.vue"

export default {
  name: 'App',
  // components: {
  //   Frank
  // }
}
</script>
