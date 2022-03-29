<template>
  <div>
    <div class="hero bg-cover rounded-lg">
      <div class="hero-overlay rounded-lg">
        <div class="text-6xl text-white font-bold w-4/6 p-28">
          <p style="letter-spacing: 1px">
            {{ text }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeroCard',
  props: {
    text: {
      type: String,
      default: '',
      required: true,
    },
  },
}
</script>
