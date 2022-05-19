<template>
  <div class="jumbotron">
    <img :src="require(`../assets/img/${img}`)" alt="">
  </div>
</template>

<script>
export default {
  name: "AppJumbotron",
  props: {
    img: String,
  },
}
</script>

<style lang="scss" scoped>

.jumbotron{
  height: 15rem;
  object-fit: contain;
  object-position: center;
  overflow: hidden;
  /* background-image: url(../assets/img/jumbotron.jpg); */
  /* background-position: center top;
  background-size: cover;
  background-repeat: no-repeat; */

  img {
    width: 100%;
  }
}
</style>