<template>
  <div class="card">
    <div class="img-wrapper">
      <img :src="comicObj.thumb" :alt="comicObj.series" />
    </div>

    <div class="card-text">
      <h4>{{ comicObj.series }}</h4>
    </div>
  </div>
</template>

<script>
export default {
  name: "ComicsCard",
  props: {
    comicObj: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
@import "../style/common.scss";

img {
  width: 100%;
  height: auto;
}

.card {
  padding: 0 5px;
  width: calc((100% / 6));
  margin-bottom: 10px;

  .img-wrapper {
    width: 100%;
    height: 0;
    padding-bottom: 100%;
    object-fit: cover;
    object-position: top;
    overflow: hidden;
  }

  .card-text {
    color: white;
    text-transform: uppercase;
    font-size: 0.8rem;
    margin-top: 10px;
  }
}
</style>