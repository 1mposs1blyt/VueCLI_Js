<template>
  <div>
    <test-component></test-component>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Test from "./components/test.vue";
export default {
  name: "App",
  components: {
    "test-component": Test,
  },
};
</script>

<style lang="less">
</style>
