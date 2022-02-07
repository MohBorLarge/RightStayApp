<template>
  <div>
    <HeroCard />
    <div class="mt-20 mb-24 flex justify-between">
      <p class="w-64 text-2xl">We are already all around Lagos.</p>
      <button class="w-36 h-12 bg-gradient-to-r from-green-200 to-green-300 text-white rounded">View All Houses</button>
    </div>
    <HouseView />
    <!-- <div class="text-center text-2xl mb-12 mx-auto">
      <a href="#" class="text-green-400 hover:text-green-700"
        >View All Houses</a
      >
    </div> -->
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
