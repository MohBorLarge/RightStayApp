<template>
  <div>
    <HeroCard />
    <AboutUs />
    <hr />
    <MissionStats />
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
