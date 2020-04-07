<template>
  <div id="app">
    <easy-bank />
  </div>
</template>

<script>
import EasyBank from "./components/easy-bank.vue";

export default {
  name: "App",
  components: {
    EasyBank
  }
};
</script>
<style lang="scss">
@import "./SCSS_Variables/styles.scss";
</style>
