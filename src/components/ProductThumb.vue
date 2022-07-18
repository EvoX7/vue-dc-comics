<template>
  <div class="thumb_wrapper">
    <div
      class=" container_imgs"
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
    text-align: center;
    padding:10px;
    text-transform: uppercase;
}
</style>