<template>
  <div>
    <HeroCard />
    <CityShow />
    <HouseView />
  </div>
</template>

<script>
import HeroCard from '@/components/homepage/HeroCard.vue'
import HouseView  from '@/components/shared/HouseView.vue'
import CityShow  from '@/components/shared/CityShow.vue'


export default {
  name: 'AllHouse',
  components: {
    HeroCard,
    HouseView,
    CityShow
  },
  layout: 'DefaultLayout',
}
</script>
