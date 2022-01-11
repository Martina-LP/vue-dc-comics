<template>
  <div class="card"> 
    <img class="card-img" :src="image" alt="Series">
    <h6 class="card-title">{{ title.toUpperCase() }}</h6>
  </div>
</template>

<script>
export default {
  props: {
    image: String,
    title: String,
  }
}
</script>

<style lang="scss">
.card {
  width: calc(100% /6); 
  margin-top: 32px;
  padding: 0 5px;

  .card-img {
    height: 160px;
    width: 160px;
    object-fit: cover;
    object-position: top;
  }

  .card-title {
    margin-top: 12px;
    font-size: 12px;
    color: lightgrey;
    font-weight: 400;
  }
}
</style>