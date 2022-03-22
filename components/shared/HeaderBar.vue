<template>
  <div>
    <header class="flex items-center mt-8 mb-12 justify-between">
      <nuxt-link to="/">
        <img
          src="@/assets/RightHomeLogo/svg/bluegreen.svg"
          alt=""
          class="w-1/6 "
        />
      </nuxt-link>
      <ul class="flex justify-between cursor-pointer text-lg font-semibold w-3/12">
        <li class="hover:text-green-400">
          <nuxt-link to="/all-houses">Short Lets</nuxt-link>
        </li>
        <li class="hover:text-green-400">
          <nuxt-link to="/about-RightHome">About RightHome</nuxt-link>
        </li>
      </ul>
    </header>
  </div>
</template>
<script>
export default {
  name: 'HeaderBar',
  data() {
    return {
      headerLinks: {
        home: 'https://github.com/johnpapa/vue-getting-started',
      },
    }
  },
  methods: {},
}
</script>
