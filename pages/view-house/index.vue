<template>
  <div>
    <CityShow />
    <HouseView />
  </div>
</template>

<script>
import HouseView from '@/components/shared/HouseView.vue'
import CityShow from '@/components/shared/CityShow.vue'


export default {
  name: 'HomePage',
  components: {
    HouseView, CityShow
  },
  layout: 'DefaultLayout',
}
</script>
