<template>
  <div class="py-20">
    <div class="pb-20 text-center">
      <p class="text-3xl font-bold mb-6">
        Select from our most popular locations
      </p>
      <div>
        <a
          v-for="(item, index) in filterItems"
          :key="index"
          class="filter-card mx-2 rounded-full px-4 py-2 cursor-pointer"
        >
          {{ item.text }}
        </a>
      </div>
    </div>

    <div class="grid gap-10 mb-12" :class="`grid-cols-${noOfCols}`">
      <div v-for="item in houses" :key="item" class="bg-white p-4 rounded-lg">
        <div class="pb-6">
          <img src="@/assets/images/home3.jpeg" alt="" class="rounded-lg" />
        </div>
        <p class="text-xl font-bold">3 Bedroom Semi-Detached Duplex</p>
        <div class="flex mt-4 mb-2">
          <unicon name="location-arrow" fill="limegreen" icon-style="line" class="mr-2" />
          <p>Preston Rd, Birmingham, Lekki, Lagos</p>
        </div>
        <div class="flex justify-between">
          <div class="flex">
            <unicon name="bed" class="mr-2"></unicon>
            <p>4 Beds</p>
          </div>
          <div class="flex">
            <unicon name="bath" fill="limegreen" class="mr-2"></unicon>
            <p>2 Baths</p>
          </div>
          <div class="flex">
            <unicon name="check-square" fill="limegreen" class="mr-2"></unicon>
            <p>890 sqft</p>
          </div>
        </div>
        <div class="flex justify-between items-center mt-8">
          <p class="w-1/2 text-green-500 text-2xl">$300,000</p>
          <BaseButton title="View House" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BaseButton from '@/components/base/BaseButton.vue'

export default {
  name: 'HouseView',
  components: {
    BaseButton,
  },
  props: {
    houses: {
      type: Array,
      default: () => [],
      required: true,
    },
    noOfCols: {
      type: Number,
      default: 3,
    },
  },
  data() {
    return {
      filterItems: [
        {
          text: 'Lagos',
          value: 'lagos',
        },
        {
          text: 'Abuja',
          value: 'abuja',
        },
        {
          text: 'Port Harcourt',
          value: 'ph',
        },
        {
          text: 'Lekki',
          value: 'lekki',
        },
        {
          text: 'Victoria Island',
          value: 'vi',
        },
        {
          text: 'Lekki',
          value: 'lekki',
        },
        {
          text: 'Victoria Island',
          value: 'vi',
        },
      ],
    }
  },
}
</script>
