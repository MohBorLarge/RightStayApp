<template>
  <div>
    <privacy-policy />
  </div>
</template>

<script>
import PrivacyPolicy from '@/components/shared/PrivacyPolicy.vue'

export default {
  name: 'PrivacyPolicy',
  components: {
    PrivacyPolicy,
  },
  layout: 'DefaultLayout',
}
</script>
