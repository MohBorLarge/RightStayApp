<template>
  <div>
    <hero-card
      text="Find the perfect place to stay with your family in several locations"
    />
    <about-us />
    <hr />
    <mission-stats />
  </div>
</template>

<script>
import HeroCard from '@/components/homepage/HeroCard.vue'
import AboutUs from '@/components/shared/AboutUs.vue'
import MissionStats from '@/components/shared/MissionStats.vue'

export default {
  name: 'AboutRightHome',
  components: {
    HeroCard,
    AboutUs,
    MissionStats,
  },
  layout: 'DefaultLayout',
}
</script>
