<template>
  <div>
    <HeroCard />
    <CityShow />
    <HouseView :houses="houses" />
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
  data() {
    return {
      houses: [1, 2, 3, 4, 5, 6],
    }
  },
}
</script>
