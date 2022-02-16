<template>
  <div>
    <view-house />
    <hr />
     <mission-stats />
  </div>
</template>
<script>
import MissionStats from '@/components/shared/MissionStats.vue'
import ViewHouse from '@/components/shared/ViewHouse.vue'

export default {
  name: 'SingleHousePage',
  components: {
    MissionStats,
    ViewHouse,
  },
  layout: 'DefaultLayout',
}
</script>
