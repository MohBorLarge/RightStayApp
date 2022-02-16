<template>
  <div>
    <hero-card text="Find the perfect place to stay with your family in several locations" />
    <house-view :houses="houses" />
    <hr />
    <review-section />
  </div>
</template>

<script>
import HeroCard from '@/components/homepage/HeroCard.vue'
import HouseView from '@/components/shared/HouseView.vue'
import ReviewSection from '~/components/homepage/ReviewSection.vue'

export default {
  name: 'HomePage',
  components: {
    HeroCard,
    HouseView,
    ReviewSection,
  },
  layout: 'DefaultLayout',
  data() {
    return {
      houses: [1, 2, 3, 4, 5, 6],
    }
  },
}
</script>
