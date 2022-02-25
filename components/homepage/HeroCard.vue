<template>
  <div>
    <div class="hero bg-cover rounded-lg">
      <div class="hero-overlay rounded-lg">
        <div class="text-6xl text-white font-bold w-5/6 p-28">
          <p style="letter-spacing: 1px">
            {{ text }}
          </p>
        </div>
      </div>
      <!-- <div class="bg-white w-3/5 h-20 p-4 flex justify-between">
        <form class="text-sm">
          <label class="block">Location</label>
          <input
            type="text"
            name=""
            value="London"
            class="text-green-400 w-14 border-none border-transparent"
          />
        </form>
        <form class="text-sm">
          <label class="block">Type</label>
          <input
            type="text"
            name=""
            value="Duplex"
            class="text-green-400 w-14 border-none"
          />
        </form>
        <form class="text-sm">
          <label class="block">Maximum Price</label>
          <input
            type="text"
            name=""
            value="₦5000"
            class="text-green-400 w-14 order-none"
          />
        </form>
        <div>
          <button
            class="w-24 h-10 bg-gradient-to-r from-green-200 to-green-300 text-white rounded"
          >
            Search
          </button>
        </div>
      </div> -->
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
