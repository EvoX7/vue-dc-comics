<template>
  <div class="thumb_wrapper">
    <div
      class="container_imgs"
      v-for="(product, index) in ProductsThumbnails"
      :key="index"
    >
      <img class="img-fluid" :src="thumbImg" alt="thumbnails" />
    </div>
    <h3>{{ comicSeries }}</h3>
  </div>
</template>

<script>
export default {
  props: {
    "thumbImg": String,
    "comicSeries": String,
    "comicPrice": String,
    "comicType": String,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
</style>