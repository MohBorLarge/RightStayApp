<template>
  <div>
    <header class="flex items-center mt-8 mb-12 justify-between">
      <img src="@/assets/RightStayLogo/svg/bluegreen.svg" alt="" class="w-40" />
      <ul class="w-2/5 flex justify-between">
        <li class="cursor-pointer">
          <a :href="headerLinks.homeType">Home Type</a>
        </li>
        <li class="cursor-pointer">About Us</li>
        <li class="cursor-pointer">Contact</li>
        <li class="cursor-pointer">Blog</li>
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
          homeType: "https://github.com/johnpapa/vue-getting-started"
        }
      }
    },
    methods: {
      
    }
  }
</script>
