<template>
  <div>
    <LargeCardDisplay
      v-for="cardSections in largeCardSections"
      :key="cardSections.id"
      :cardsSection="cardSections"
    />
    <SmallCardDisplay
      v-for="cardSections in smallCardSections"
      :key="cardSections.id"
      :cardsSection="cardSections"
    />
  </div>
</template>

<script>
import { largeCardSections, smallCardSections } from '@/assets/data.js'
export default {
  data () {
    return {
      largeCardSections, smallCardSections
    }
  }
}
</script>
