<template>
  <footer>
    <div id="dc-heroes">
      <div class="container d-flex">
        <nav id="footer-nav">
          <div id="left-column-footer">
            <!-- DC COMICS  -->
            <ul>
              <h4 class="text-uppercase text-white">dc comics</h4>
              <li v-for="(comic, index) in dcComics" :key="index">
                <a :href="comic.url">{{ comic.text }}</a>
              </li>
            </ul>

            <!-- SHOP -->
            <ul>
              <h4 class="text-uppercase text-white">shop</h4>
              <li v-for="(item, index) in shop" :key="index">
                <a :href="item.url">{{ item.text }}</a>
              </li>
            </ul>
          </div>

          <div id="central-column-footer">
            <!-- DC  -->
            <ul>
              <h4 class="text-uppercase text-white">dc</h4>
              <li v-for="(policy, index) in DC" :key="index">
                <a :href="policy.url">{{ policy.text }}</a>
              </li>
            </ul>
          </div>
          <div id="right-column-footer">
            <!-- SITES  -->
            <ul>
              <h4 class="text-uppercase text-white">sites</h4>
              <li v-for="(site, index) in sites" :key="index">
                <a :href="site.url">{{ site.text }}</a>
              </li>
            </ul>
          </div>
        </nav>
      </div>
      <div id="dc-logo-bg">
        <img src="../assets/img/dc-logo-bg.png" alt="dc-logo-bg" />
      </div>
    </div>

    <div
      class="container d-flex justify-content-between align-items-center"
      id="sub-footer1"
    >
      <div
        class="text-uppercase d-flex align-items-center justify-content-center"
        id="btn-signup"
      >
        <a
          class="text-decoration-none text-white"
          href="https://www.dccomics.com/newsletter"
        >
          <span> Sign-Up now!</span></a
        >
      </div>
      <div id="footer-socials">
        <span class="text-uppercase fw-bold fs-4 px-4" id="follow"
          >Follow us</span
        >
        <a class="social-hover" href="https://www.facebook.com/dc">
          <img
            class="px-3"
            src="../assets/img/footer-facebook.png"
            alt="facebook"
        /></a>
        <a class="social-hover" href="https://twitter.com/dccomics">
          <img src="../assets/img/footer-twitter.png" alt="twitter"
        /></a>
        <a href="http://www.youtube.com/user/DCEntertainmentTV">
          <img
            class="px-3"
            src="../assets/img/footer-youtube.png"
            alt="youtube"
        /></a>
        <a class="social-hover" href="http://www.pinterest.com/dccomics/">
          <img
            class="px-1"
            src="../assets/img/footer-pinterest.png"
            alt="pinterest"
        /></a>
        <a class="social-hover" href="https://www.periscope.tv/DCComics">
          <img
            class="px-3"
            src="../assets/img/footer-periscope.png"
            alt="periscope"
        /></a>
      </div>
    </div>

    <div id="bottom-footer"></div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data: function () {
    return {
      dcComics: [
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
          text: "TV",
          url: "/#",
        },
        {
          text: "Games",
          url: "/#",
        },
        {
          text: "Videos",
          url: "/#",
        },
        {
          text: "News",
          url: "/#",
        },
      ],
      shop: [
        {
          text: "Shop DC",
          url: "/#",
        },
        {
          text: "Shop DC Collectibles",
          url: "/#",
        },
      ],
      DC: [
        {
          text: "Terms Of Use",
          url: "/#",
        },
        {
          text: "Privacy policy",
          url: "/#",
        },
        {
          text: "Ad Choices",
          url: "/#",
        },
        {
          text: "Advertising",
          url: "/#",
        },
        {
          text: "Jobs",
          url: "/#",
        },
        {
          text: "Subscriptions",
          url: "/#",
        },
        {
          text: "Talent Workshops",
          url: "/#",
        },
        {
          text: "CPSC Certificates",
          url: "/#",
        },
        {
          text: "Ratings",
          url: "/#",
        },
        {
          text: "Shop Help",
          url: "/#",
        },
        {
          text: "Contacts Us",
          url: "/#",
        },
      ],
      sites: [
        {
          text: "DC",
          url: "/#",
        },
        {
          text: "MAD Magazine",
          url: "/#",
        },
        {
          text: "DC Kids",
          url: "/#",
        },
        {
          text: "DC Universe",
          url: "/#",
        },
        {
          text: "DC Power Visa",
          url: "/#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

footer {
  position: relative;
  background-color: $brandTertiary;

  #sub-footer1 {
    background-color: $brandTertiary;
    height: 100px;
  }

  #dc-heroes {
    height: 380px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: 1950px;
    overflow: hidden;
  }

  #dc-logo-bg {
    float: right;
    position: relative;
    right: 260px;
    bottom: 450px;
  }

  #btn-signup {
    border: 2px solid $brandPrimary;
    background-color: transparent;
    width: 150px;
    height: 50px;
    font-size: 17px;
    font-weight: bold;
    cursor: pointer;
    transition: 0.3s;

    &:hover {
      background-color: $brandPrimary;
    }
  }

  li {
    list-style: none;
  }

  a {
    text-decoration: none;
    color: rgb(139, 139, 139);

    &:hover {
      color: $brandPrimary;
    }
  }

  #follow {
    font-family: "Yanone Kaffeesatz", sans-serif;
    color: $brandPrimary;
  }

  #footer-socials {
    display: flex;
    align-content: center;
  }

  #bottom-footer {
    background-color: #222222;
    height: 20px;
  }

  #footer-nav {
    text-align: left;
    margin-top: 50px;
    display: flex;
    font-family: "Yanone Kaffeesatz", sans-serif;
  }
}
</style>