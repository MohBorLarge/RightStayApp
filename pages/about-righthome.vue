<template>
  <div>
    <hero-card
      text="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod"
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
  name: 'AboutRightStay',
  components: {
    HeroCard,
    AboutUs,
    MissionStats,
  },
  layout: 'DefaultLayout',
}
</script>
