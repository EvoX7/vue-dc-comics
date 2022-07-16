<template>
  <main>
    <div class="d-flex justify-content-center align-items-center" id="banner-top">
        <h1>Batman forever</h1>
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
    height: 140px;
  }
 

  h1 {
    color: yellow;
  }

  h2 {
    color: rgb(255, 255, 255);
  }

</style>