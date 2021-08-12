<template>
  <div class="container">
    <h4 class="header">
      {{ cardsSection.title }}
    </h4>
    <div class="cards-container">
      <b-row>
        <SmallCard
          v-for="card in cardsSection.cards"
          :key="card.id"
          :card="card"
        />
      </b-row>
    </div>
  </div>
</template>

<script>
export default {
  props: ['cardsSection']
}
</script>

<style scoped>
  .container {
    padding: 2rem 0
  }
  .header {
    font-weight: 700;
    font-size: 1.5rem;
    margin-bottom: 2rem;
  }
  .card-container {
    /* display: flex; */
    justify-content: space-between;
    flex-wrap: wrap;
  }
</style>
