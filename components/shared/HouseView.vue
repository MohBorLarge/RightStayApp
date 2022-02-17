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
      <div
        v-for="(item, index) in houses"
        :key="index"
        class="bg-white p-4 rounded-lg"
      >
        <div class="pb-6">
          <img src="@/assets/images/home3.jpeg" alt="" class="rounded-lg" />
        </div>
        <p class="text-xl font-bold">{{ item.houseTitle }}</p>
        <div class="flex mt-4 mb-2">
          <navigation-2-icon
            size="1.2x"
            class="custom-class"
          ></navigation-2-icon>
          <p>{{ item.houseAddress }}, {{ item.state }}</p>
        </div>
        <div class="flex justify-between">
          <div class="flex">
            <hard-drive-icon
              size="1.5x"
              class="custom-class mr-2"
            ></hard-drive-icon>
            <p>{{ item.noOfBedrooms }} Beds</p>
          </div>
          <div class="flex">
            <hard-drive-icon
              size="1.5x"
              class="custom-class mr-2"
            ></hard-drive-icon>
            <p>{{ item.noOfBathrooms }} Baths</p>
          </div>
          <div class="flex">
            <square-icon size="1.3x" class="custom-class mr-2"></square-icon>
            <p>{{ item.squareFeet }} Sqft.</p>
          </div>
        </div>
        <div class="flex justify-between items-center mt-8">
          <p class="w-1/2 text-green-500 text-2xl">$300,000</p>
          <BaseButton
            title="View House"
            :link="`/single-house/${item.houseId}`"
          />
        </div>
      </div>
    </div>

    <div v-if="showViewAllBtn" class="text-center w-full my-8">
      <BaseButton title="View all houses" link="/all-houses" />
    </div>
  </div>
</template>

<script>
import { HardDriveIcon, Navigation2Icon, SquareIcon } from 'vue-feather-icons'
import BaseButton from '@/components/base/BaseButton.vue'

export default {
  name: 'HouseView',
  components: {
    BaseButton,
    HardDriveIcon,
    Navigation2Icon,
    SquareIcon,
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
    showViewAllBtn: {
      type: Boolean,
      default: true,
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
