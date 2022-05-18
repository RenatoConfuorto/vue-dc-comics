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

    <footer>
      <AppFooter/>
    </footer>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppContent from "./components/AppContent.vue";
import AppIcons from "./components/AppIcons.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppContent,
    AppIcons,
    AppFooter,
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
