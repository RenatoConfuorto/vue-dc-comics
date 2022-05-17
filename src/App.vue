<template>
  <div id="app">
    <!-- header -->
    <header>
      <AppHeader/>
    </header>

    <!-- main -->
    <main>
      <AppContent/>
      <AppIcons/>
    </main>
    <!-- footer -->
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppContent from "./components/AppContent.vue";
import AppIcons from "./components/AppIcons.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppContent,
    AppIcons,
  },
  created(){
    document.title = 'Dc - Comics'
  }
}
</script>

<style lang="scss">
  @import "./style/variables.scss";
  @import "./style/common.scss";
</style>
