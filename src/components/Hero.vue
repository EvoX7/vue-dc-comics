<template>
  <div class="" id="hero">
    <div class="internal-container">
      <img
        src="../assets/img/buy-comics-digital-comics.png"
        alt="digital-comics"
      />
      <span class="px-2 me-5 text-white">DIGITAL COMICS</span>
      <img src="../assets/img/buy-comics-merchandise.png" alt="merchandise" />
      <span class="px-2 me-5 text-white">DC MERCHANDISE</span>
      <img
        src="../assets/img/buy-comics-subscriptions.png"
        alt="subscriptions"
      />
      <span class="px-2 me-5 text-white">SUBSCRIPTION</span>
      <img src="../assets/img/buy-comics-shop-locator.png" alt="shop-locator" />
      <span class="px-2 me-5 text-white">COMIC SHOP LOCATOR</span>
      <img src="../assets/img/buy-dc-power-visa.svg" alt="shop-locator" />
      <span class="px-2 me-5 text-white">DC POWER VISA</span>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

#hero {
  display: flex;
  align-content: center;
  justify-content: center;
  padding: 60px;
  background-color: $brandPrimary;

  img {
    width: 50px;
    height: 55px;
  }
}
</style>

