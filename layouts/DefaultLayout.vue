<template>
  <div>
    <div class="container">
      <header-bar />
      <nuxt />
    </div>
    <whats-app class="pb-12"/>
    <footer-section />
  </div>
</template>

<script>
import HeaderBar from '@/components/shared/HeaderBar.vue'

import FooterSection from '@/components/shared/FooterSection.vue'
import WhatsApp from '@/components/shared/WhatsApp.vue'

export default {
  name: 'DefaultLayout',
  components: {
    HeaderBar, FooterSection,
    WhatsApp
  },
  data() {
    return {
      
    }
  }
}
</script>
