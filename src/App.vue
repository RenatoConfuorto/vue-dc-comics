<template>
  <div id="app">
    <!-- header -->
    <header>
      <AppHeader/>
    </header>

    <!-- main -->
    <main>
      <AppJumbotron/>
    </main>
    <!-- footer -->

    <footer>
      <AppIcons/>
      <AppFooter/>
      <AppFooterAction/>
    </footer>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppIcons from "./components/AppIcons.vue";
import AppFooter from "./components/AppFooter.vue";
import AppFooterAction from "./components/AppFooterAction.vue";
import AppJumbotron from "./components/AppJumbotron.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppIcons,
    AppFooter,
    AppFooterAction,
    AppJumbotron,
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
