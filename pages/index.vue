<template>
  <div>
    <HeroCard />
    <CityShow />
    <HouseView :no-of-rows="2" />
  </div>
</template>

<script>
import HeroCard from '@/components/homepage/HeroCard.vue'
import HouseView from '@/components/shared/HouseView.vue'
import CityShow from '@/components/shared/CityShow.vue'

export default {
  name: 'HomePage',
  components: {
    HeroCard,
    HouseView,
    CityShow,
  },
  layout: 'DefaultLayout',
}
</script>
