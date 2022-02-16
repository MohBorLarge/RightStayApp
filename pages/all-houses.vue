<template>
  <div>
    <house-view :houses="houses" />
    <hr />
    <mission-stats />
  </div>
</template>

<script>
import HouseView from '@/components/shared/HouseView.vue'
import MissionStats from '@/components/shared/MissionStats.vue'

export default {
  name: 'AllHouses',
  components: {
    HouseView,
    MissionStats,
  },
  layout: 'DefaultLayout',
  data() {
    return {
      houses: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],
    }
  },
}
</script>
