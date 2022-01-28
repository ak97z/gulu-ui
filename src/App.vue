<template>
  <div>
    导航栏
    <router-link to="/">Home</router-link>
    <router-link to="/doc">Doc</router-link>
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
