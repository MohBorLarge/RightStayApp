<template>
  <div class="flex">
    <p v-if="!fullScreen" class="text-green-400 w-3/6 mt-8 mr-24 text-xl">
      Lagos State
    </p>
    <div class="grid gap-10 mb-12" :class="`grid-cols-${noOfCols}`">
      <div v-for="item in houses" :key="item" class="bg-white p-4 rounded-lg">
        <div class="pb-6">
          <img src="@/assets/images/home3.jpeg" alt="" class="rounded-lg" />
        </div>
        <div class="text-xl mb-2">
          <p class="text-green-400">$300,000</p>
        </div>
        <div class="location flex text-gray-400">
          <div>
            <LocationSharp
              class="text-gray-400 h-4"
              style="margin: 3px 2px 0 0"
            />
          </div>
          <p>Preston Rd, Birmingham</p>
        </div>
        <div class="details flex justify-between">
          <div class="flex text-gray-400">
            <BedOutline class="h-4" style="margin: 3px 3px 0 0" />
            <p>4 Bd.</p>
          </div>
          <div class="flex text-gray-400">
            <SBath class="h-4" style="margin: 3px 3px 0 0" />
            <p>2 Ba.</p>
          </div>
          <div class="flex text-gray-400">
            <SquareSharp class="h-4" style="margin: 3px 3px 0 0" />
            <p>890 sqft.</p>
          </div>
        </div>
        <nuxt-link to="/single-house">
          <button
            class="bg-green-600 hover:bg-green-700 text-white py-2 w-full mt-4 text-center rounded-md"
          >
            View House
          </button>
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HouseView',
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
    fullScreen: {
      type: Boolean,
      default: false,
    },
  },
}
</script>
