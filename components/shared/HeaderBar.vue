<template>
  <div>
    <header class="flex items-center mt-8 mb-12 justify-between">
      <img src="@/assets/RightStayLogo/svg/bluegreen.svg" alt="" class="w-40" />
      <ul class="w-2/5 flex justify-between text-green-400 cursor-pointer">
        <li>
          <nuxt-link to="/">Home</nuxt-link>
        </li>
        <li>
          About Us
        </li>
        <li>Contact</li>
        <li>Blog</li>
        <li>Buy Property</li>
      </ul>
    </header>
  </div>
</template>
<script>
  export default {
    name: "HeaderBar",
    data() {
      return {
        headerLinks: {
          home: "https://github.com/johnpapa/vue-getting-started"
        }
      }
    },
    methods: {
      
    }
  }
</script>
