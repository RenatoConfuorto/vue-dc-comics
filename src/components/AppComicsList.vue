<template>
  <div class="comics-list">
    <div class="container">
      <h2 class="series">Current series</h2>

      <div class="card-container">
        <ComicsCard v-for="(item, index) in comicsList" :key="index" :comicObj="item"/>
      </div>

      <button class="load-btn">Load More</button>
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
@import "../style/variables.scss";
@import "../style/common.scss";

.comics-list{
  padding: 3rem 0;

  

  .container{
    position: relative;
    text-align: center;

    .series{
      position: absolute;
      top: -4rem;
      color: white;
      text-transform: uppercase;
      font-size: 1.3rem;
      padding: 0.3rem 0.8rem;
      background-color: $brand-color;
    }

    .card-container{
      display: flex;
      flex-wrap: wrap;
      margin-bottom: 1.5rem;
    }
  
    .load-btn{
      text-transform: uppercase;
      font-size: 0.8rem;
      color: white;
      background-color: $brand-color;
      padding: 0.4rem 0.8rem;
      border: 0;
      min-width: 10rem;
      cursor: pointer;
    }
  }
}

</style>