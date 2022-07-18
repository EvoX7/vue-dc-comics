<template>
  <div class="thumb_wrapper">
    <div
      class="container_imgs ">
      <img :src="thumbImg" alt="thumbnails" />
    </div>
    <h6 class="text-wrap">{{ comicSeries }}</h6>
    
   
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



img {
    width: 200px;
    height: 200px;
    padding: 10px;
    object-fit: cover;
    object-position: top;
    cursor: pointer;
    transition: 0.3s;

    &:hover {
        transform: scale(1.1);
        
    }
    
}

h6 {
  padding:5px;
    text-align: center;
    text-transform: uppercase;
    
}
</style>