<template>
  <div class="container">
    <h2> &rarr; Content goes here &larr; </h2>
  </div>
</template>

<script>
export default {
  
}
</script>

<style lang="scss" scoped>
  @import "../style/variables.scss";
  @import "../style/common.scss";

.container{
  height: $app-content-height;
  color: white;
  font-size: 1.3rem;
  line-height: $app-content-height;
}

</style>