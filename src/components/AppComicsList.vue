<template>
  <div class="comics-list">
    <div class="container">
      <ComicsCard v-for="(item, index) in comicsList" :key="index" :comicObj="item"/>
    </div>
  </div>
</template>

<script>
import ComicsCard from "./ComicsCard.vue";

export default {
  data() {
    return{
      //array dei fumetti
      comicsList: require('../assets/dc-comics.json'),
    }
  },
  components: {
    ComicsCard,
  }

}
</script>

<style lang="scss" scoped>

.comics-list{
  padding: 3rem 0;

  .container{
    display: flex;
    flex-wrap: wrap;
  
  }
}

</style>