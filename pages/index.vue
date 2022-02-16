<template>
  <div>
    <hero-card
      text="Find the perfect place to stay with your family in several locations"
    />
    <house-view :houses="houses" />
    <hr />
    <review-section />
  </div>
</template>

<script>
import HeroCard from '@/components/homepage/HeroCard.vue'
import HouseView from '@/components/shared/HouseView.vue'
import ReviewSection from '~/components/homepage/ReviewSection.vue'

import client from '~/plugins/contentful'

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
      houses: [],
    }
  },
  async created() {
    const response = await client.getEntries({
      content_type: 'houseTitle',
    })
    this.houses = response.items
      .slice()
      .reverse()
      .map((item) => console.log('checking here', item))
  },
}
</script>
