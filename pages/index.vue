<template>
  <div>
    <Hero />
    <LargeCardDisplay
      v-for="cardSections in largeCardSections"
      :key="cardSections.id"
      :cardsSection="cardSections"
    />
  </div>
</template>

<script>
import { largeCardSections } from '@/assets/data.js'
export default {
  data () {
    return {
      largeCardSections
    }
  }
}
</script>
