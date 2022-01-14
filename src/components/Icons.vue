<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="card">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="Comics">
          <span>DIGITAL COMICS</span>
        </div>
        <div class="card">
          <img src="../assets/img/buy-comics-merchandise.png" alt="Merchandise">
          <span>DC MERCHANDISE</span>
        </div>
        <div class="card">
          <img src="../assets/img/buy-comics-subscriptions.png" alt="Subscriptions">
          <span>SUBSCRIPTION</span>
        </div>
        <div class="card">
          <img src="../assets/img/buy-comics-shop-locator.png" alt="Shop Locator">
        <span>COMIC SHOP LOCATOR</span>
        </div>
        <div class="card">
          <img src="../assets/img/buy-dc-power-visa.svg" alt="Power Visa">
          <span>DC POWER VISA</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Icons'
}
</script>

<style scoped lang="scss">
@import '../style/variables';

section {
  background-color: $primary_color;
  height: 150px;

  .row {
    display: flex;
    height: 120px;
    padding: 0 16px;
    justify-content: space-between;
    align-items: center;
  
    .card {
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
      cursor: pointer;

      img {
        width: 40px;
        margin: 10px;
      }

      span {
        font-size: 15px;
      }
    }
  } 
}

</style>