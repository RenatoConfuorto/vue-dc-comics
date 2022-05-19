<template>
  <div id="app">
    <!-- header -->
    <header>
      <AppHeader/>
    </header>

    <!-- main -->
    <main>
      <AppJumbotron :img="jumbo1"/>
      <AppComicsList/>
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
import AppComicsList from "./components/AppComicsList.vue";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppIcons,
    AppFooter,
    AppFooterAction,
    AppJumbotron,
    AppComicsList,
  },
  data(){
    return{
      jumbo1: 'jumbotron.jpg'
    }
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
