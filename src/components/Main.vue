<template>
  <main>
    <div class="d-flex justify-content-center align-items-center" id="banner-top">
        <h1>Batman forever</h1>
    </div>
    <div class="d-flex justify-content-center align-items-center" id="banner-bottom">
        <h2>Wonder woman too!</h2> 
         
    </div>
    
  </main>
  
</template>

<script>
export default {
  name: "Main",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";



  #banner-top {
    background-color: $brandSecondary;
    height: 120px;
  }
  #banner-bottom {
    background-color: $brandPrimary;
    height: 150px;
  }

  h1 {
    color: yellow;
  }

  h2 {
    color: rgb(255, 255, 255);
  }

</style>