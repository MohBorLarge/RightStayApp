<template>
  <div class="footer text-white px-12 sm:px-0">
    <div class="container">
      <div class="flex py-24">
        <div class="w-2/4 text-3xl font-bold pr-16">
          <p class="mb-4">Lekky County Homes, Ikota, Lekki, Lagos</p>
          <p class="mb-4">+234 8098551970 & +234 8181389018</p>
          <a href="mailto@info@righthome.ng" class="color-green"
            >info@righthome.ng</a
          >
        </div>
        <div class="w-1/4 text-xl">
          <ul>
            <li>
              <nuxt-link to="/all-houses">Short Lets</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/about-RightHome">About RightHome</nuxt-link>
            </li>
            <li>
              <nuxt-link to="/terms-conditions"
                >Term &amp; Conditions</nuxt-link
              >
            </li>
          </ul>
        </div>
        <div class="w-1/4 text-xl">
          <ul>
            <li class="flex items-center">
              <twitter-icon size="1x" class="custom-class mr-4"></twitter-icon>
              <a href="https://www.twitter.com">Twitter</a>
            </li>
            <li class="flex items-center">
              <facebook-icon
                size="1x"
                class="custom-class mr-4"
              ></facebook-icon>
              <a href="https://www.facebook.com">Facebook</a>
            </li>
            <li></li>
            <li class="flex items-center">
              <instagram-icon
                size="1x"
                class="custom-class mr-4"
              ></instagram-icon>
              <a href="https://www.instagram.com/righthomeng/">Instagram</a>
            </li>
          </ul>
        </div>
      </div>
      <hr style="border-color: white" />
      <div class="pb-12 text-center mt-12 text-xl">
        <p>
          © {{ new Date().getFullYear() }}
          <strong class="font-black">RightHome</strong>. All right reserved
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import { TwitterIcon, FacebookIcon, InstagramIcon } from 'vue-feather-icons'

export default {
  name: 'FooterSection',
  components: { TwitterIcon, FacebookIcon, InstagramIcon },
  data() {
    return {}
  },
}
</script>

<style scoped>
ul li {
  margin: 1rem 0;
}
ul li:first-child {
  margin-top: 0;
}
ul li:last-child {
  margin-bottom: 0;
}
</style>
