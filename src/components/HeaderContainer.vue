<template>
  <header>
    <div class="" id="top-bar"></div>
    <nav class="container d-flex align-items-center justify-content-between">
      <div>
        <a href="https://www.dccomics.com/"
          ><img id="logo" src="../assets/img/dc-logo.png" alt="dclogo"
        /></a>
      </div>
      <ul class="d-flex me-5 pe-5">
        <li v-for="(link, index) in navBar" :key="index">
          <a :href="link.url">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",

  data: function () {
    return {
      navBar: [
        {
          text: "Characters",
          url: "/#",
        },
        {
          text: "Comics",
          url: "/#",
        },
        {
          text: "Movies",
          url: "/#",
        },
        {
          text: "Tv",
          url: "/#",
        },
        {
          text: "Games",
          url: "/#",
        },
        {
          text: "Collectibles",
          url: "/#",
        },
        {
          text: "Videos",
          url: "/#",
        },
        {
          text: "Fans",
          url: "/#",
        },
        {
          text: "News",
          url: "/#",
        },
        {
          text: "Shop",
          url: "/#",
        },
      ],
    };
  },
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
    letter-spacing: 3px;
    list-style: none;
    padding: 0px 9px;
    border-bottom: 2px solid transparent;
    transition: 0.3s;

    &:hover {
      border-bottom: 2px solid $brandPrimary;
    }
  }

  a {
    text-decoration: none;
    color: rgb(0, 0, 0);

    &:hover {
      color: $brandPrimary;
    }
  }
}
</style>