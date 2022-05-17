<template>
  <div id="app">
    <!-- header -->
    <header>
      <AppHeader/>
    </header>

    <!-- main -->
    <main>
      <AppContent/>
    </main>
    <!-- footer -->
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppContent from "./components/AppContent.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppContent,
  }
}
</script>

<style lang="scss">
  @import "./style/variables.scss";
  @import "./style/common.scss";
</style>
