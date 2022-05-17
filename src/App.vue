<template>
  <div id="app">
    <!-- header -->
    <header>
      <AppHeader/>
    </header>

    <!-- main -->

    <!-- footer -->
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
  }
}
</script>

<style lang="scss">
  @import "./style/variables.scss";
  @import "./style/common.scss";
</style>
