<template>
  <div id="blue-banner">
    <div
      id="internal-container"
      v-for="(product, index) in products"
      :key="index"
    >
      <a :href="product.url_2">
        <img :src="product.url" :alt="product.text" />
        <span id="products-text">{{ product.text }}</span></a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: "BlueBanner",

  data: function () {
    return {
      products: [
        {
          text: "Digital Comics",
          url: require("../assets/img/buy-comics-digital-comics.png"),
          url_2: "http://www.dcuniverseinfinite.com/",
        },
        {
          text: "DC Merchandise",
          url: require("../assets/img/buy-comics-merchandise.png"),
          url_2: "https://shop.dccomics.com/",
        },
        {
          text: "Subscription",
          url: require("../assets/img/buy-comics-subscriptions.png"),
          url_2: "https://subscriptions.dccomics.com/",
        },
        {
          text: "Comic Shop locator",
          url: require("../assets/img/buy-comics-shop-locator.png"),
          url_2: "https://www.dccomics.com/ComicShopLocator",
        },
        {
          text: "DC Power visa",
          url: require("../assets/img/buy-dc-power-visa.svg"),
          url_2: "http://www.dcuniverseinfinite.com/",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

#blue-banner {
  display: flex;
  align-content: center;
  justify-content: center;
  padding: 20px;
  background-color: $brandPrimary;

  #internal-container {
    padding: 30px;
    cursor: pointer;
  }

  img {
    width: 50px;
    height: 55px;

    &:hover {
      transform: rotate(10deg);
    }
  }

  a {
    text-decoration: none;
  }

  #products-text {
    text-transform: uppercase;
    color: white;
    padding-left: 20px;
  }
}
</style>

