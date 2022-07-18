<template>
  <div class="thumb_wrapper">
    <div
      class="container_imgs"
      :key="index">
      <img :src="thumbImg" alt="thumbnails" />
    </div>
    <h6>{{ comicSeries }}</h6>
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

.container_imgs {
    margin-top:50px;
   
    
}

h6 {
    text-transform: uppercase;
}
</style>