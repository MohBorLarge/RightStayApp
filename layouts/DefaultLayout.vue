<template>
  <div>
    <div class="container">
      <HeaderBar />
      <nuxt />
    </div>
    <FooterSection />
  </div>
</template>

<script>
import HeaderBar from '@/components/shared/HeaderBar.vue'
import FooterSection from '@/components/shared/FooterSection.vue'

export default {
  name: 'DefaultLayout',
  components: {
    HeaderBar, FooterSection
  },
  data() {
    return {
      
    }
  }
}
</script>
