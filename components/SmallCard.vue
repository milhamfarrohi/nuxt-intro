<template>
  <b-col class="card-col" sm="3">
    <nuxt-link :to="`/products/${card.id}`" class="card-container">
      <img class="image" :src="require(`@/assets/images/${card.image || 'fe1.jpg'}`)" alt="">
    </nuxt-link>
  </b-col>
</template>

<script>
export default {
  props: ['card']
}
</script>

<style scoped>
  .card-col {
    margin-bottom: 1.5rem;
    border-radius: 0.5rem;
  }
  .card-container {
    width: 24%;
    height: 12.5rem;
    border-radius: 0.5rem;
    overflow: hidden;
    margin-bottom: 1.5rem;
    cursor: pointer;
  }
  .image {
    border-radius: 0.5rem;
    width: 100%;
    max-height: 208px;
  }
</style>
