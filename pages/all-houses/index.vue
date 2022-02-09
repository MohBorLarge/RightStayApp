<template>
  <div>
    <CityShow :show-button="false" />
    <HouseView :no-of-rows="4" :full-screen="true" />
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
}
</script>
