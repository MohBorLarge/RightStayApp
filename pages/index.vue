<template>
  <div>
    <HeroCard />
    <div class="mt-20 mb-24">
      <p class="w-64 text-2xl">We are already all around Lagos.</p>
    </div>
    <div class="text-center text-2xl my-12 mx-auto">
      <a href="#" class="text-green-400 hover:text-green-700"
        >View All Houses</a
      >
    </div>
    <HouseView />
  </div>
</template>

<script>
import HeroCard from '@/components/homepage/HeroCard.vue'
import HouseView from '@/components/shared/HouseView.vue'

export default {
  name: 'HomePage',
  components: {
    HeroCard,
    HouseView,
  },
  layout: 'DefaultLayout',
}
</script>
