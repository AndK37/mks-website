<template>
  <my-header></my-header>
  <router-view />
  <my-footer></my-footer>
</template>

<script>
import MyHeader from "../src/components/MyHeader.vue";
import MyFooter from "../src/components/MyFooter.vue";

export default {
  components: {
    "my-header": MyHeader,
    "my-footer": MyFooter,
  }
}
</script>

<style>
body {
  margin: 0px;
  padding: 0px;
}

#app {
  margin-left: min(50px, 5%);
  margin-right: min(50px, 5%);
  
}

</style>
