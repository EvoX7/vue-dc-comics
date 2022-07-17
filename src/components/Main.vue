<template>
  <main>
    <div
      class="d-flex justify-content-center align-items-center"
      id="banner-top"
    >
      <img class="image-fluid" src="../assets/img/Batman-Logo.png" alt="batlogo">
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

img {
  width: 280px;
  height: 160px;
  
 
}
</style>