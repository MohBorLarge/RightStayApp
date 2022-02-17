<template>
  <div>
    <view-house :current-house="currentHouse" />
    <hr />
    <mission-stats />
  </div>
</template>
<script>
import MissionStats from '@/components/shared/MissionStats.vue'
import ViewHouse from '@/components/shared/ViewHouse.vue'
import client from '~/plugins/contentful'

export default {
  name: 'SingleHousePage',
  components: {
    MissionStats,
    ViewHouse,
  },

  layout: 'DefaultLayout',

  data() {
    return {
      houses: [],
      currentHouse: {},
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

    this.currentHouse = this.houses.find(
      (item) => item.houseId === this.$route.params.id
    )

    console.log('checking currentHouse', this.currentHouse)
  },
}
</script>
