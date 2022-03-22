<template>
  <div>
    <house-view :houses="houses" :show-view-all-btn="false" />
    <hr />
    <mission-stats />
  </div>
</template>

<script>
import HouseView from '@/components/shared/HouseView.vue'
import MissionStats from '@/components/shared/MissionStats.vue'
import client from '~/plugins/contentful'

export default {
  name: 'AllHouses',
  components: {
    HouseView,
    MissionStats,
  },
  layout: 'DefaultLayout',
  data() {
    return {
      houses: [],
    }
  },
  async created() {
    const response = await client.getEntries({
      content_type: 'houseTitle',
    })
    this.houses = response.items
      .slice()
      .reverse()
      .map((item) => {
        return {
          ...item.fields,
        }
      })
  },
}
</script>
