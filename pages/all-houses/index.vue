<template>
  <div>
    <CityShow :show-button="false" />
    <HouseView :houses="houses" :full-screen="true" />
  </div>
</template>

<script>
import HouseView from '@/components/shared/HouseView.vue'
import CityShow from '@/components/shared/CityShow.vue'

export default {
  name: 'AllHouses',
  components: {
    HouseView,
    CityShow,
  },
  layout: 'DefaultLayout',
  data() {
    return {
      houses: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
    }
  },
}
</script>
