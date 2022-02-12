<template>
  <div>
    <HeroCard />
    <MissionStats />
    <CityShow />
    <HouseView :houses="houses" />
    <ReviewSection />
  </div>
</template>

<script>
import HeroCard from '@/components/homepage/HeroCard.vue'
import HouseView from '@/components/shared/HouseView.vue'
import CityShow from '@/components/shared/CityShow.vue'
import ReviewSection from '~/components/homepage/ReviewSection.vue'
import MissionStats from '~/components/shared/MissionStats.vue'


export default {
  name: 'HomePage',
  components: {
    HeroCard,
    HouseView,
    CityShow,
    ReviewSection,
    MissionStats
  },
  layout: 'DefaultLayout',
  data() {
    return {
      houses: [1, 2, 3, 4, 5, 6],
    }
  },
}
</script>
