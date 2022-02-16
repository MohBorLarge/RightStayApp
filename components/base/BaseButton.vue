<template>
  <nuxt-link :to="link">
    <button class="base-button px-4 py-2 text-center rounded-lg">
      {{ title }}
    </button>
  </nuxt-link>
</template>

<script>
export default {
  name: 'BaseButton',
  props: {
    title: {
      type: String,
      default: 'Submit',
    },
    link: {
      type: String,
      default: '',
    },
  },
}
</script>
