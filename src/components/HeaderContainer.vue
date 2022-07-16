<template>
  <header>
    <div class="" id="top-bar"></div>
    <nav class="container d-flex align-items-center justify-content-between">
      <div>
        <a href="https://www.dccomics.com/"
          ><img id="logo" src="../assets/img/dc-logo.png" alt="dclogo"
        /></a>
      </div>
       <ul class="d-flex">
          <li>collectibles</li>
          <li>collectibles</li>
          <li>collectibles</li>
          <li>collectibles</li>
          <li>collectibles</li>
          <li>collectibles</li>
          <li>collectibles</li>
          <li>collectibles</li>
          <li>collectibles</li>
          <li>collectibles</li>
        </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

header {
  height: 150px;

  #top-bar {
    background-color: #212121;
    height: 20px;
  }

  nav {
    height: 130px;
    background-color: white;
    font-family: "Yanone Kaffeesatz", sans-serif;
  }

  #logo {
    width: 80px;
    height: 80px;
  }


  li {
    text-transform: uppercase;
    font-size: 17px;
    color: black;
    list-style: none;
    padding: 0px 10px;
    border-bottom: 2px solid transparent;
    cursor: pointer;
   

    &:hover {
      border-bottom: 2px solid $brandPrimary;
    }
  }
}
</style>