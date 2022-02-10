<template>
  <div class="mt-20 mb-24 flex justify-between">
    <p class="text-5xl" :class="showButton ? 'w-5/12' : 'w-7/12'">
      We are already all around Lagos.
    </p>
    <nuxt-link to="/all-houses">
      <button
        v-if="showButton"
        class="w-36 h-12 bg-gradient-to-r from-green-200 to-green-300 text-white rounded mt-4"
      >
        View All Houses
      </button>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'CityShow',
  props: {
    showButton: {
      type: Boolean,
      default: true,
    },
  },
}
</script>

<style lang="scss" scoped></style>
