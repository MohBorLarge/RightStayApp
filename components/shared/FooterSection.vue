<template>
  <div class="footer text-white">
    <div class="container">
      <div class="flex py-24">
        <div class="w-2/4 text-3xl font-bold pr-16">
          <p class="mb-4">
            59 Bervely Hill Ave, Brooklyn Town, New York, NY 5630, CA, US
          </p>
          <p class="mb-4">+056 686 56 56 98</p>
          <a href="mailto@hello@RightStay.com" class="color-green"
            >hello@rightsource.com</a
          >
        </div>
        <div class="w-1/4 text-xl">
          <ul class="flex justify-between">
            <li class="flex">
              <twitter-icon size="1x" class="custom-class"></twitter-icon>
              <a href="about-us.html">Twitter</a>
            </li>
            <li class="flex">
              <facebook-icon size="1x" class="custom-class"></facebook-icon>
              <a href="about-us.html">Facebook</a>
            </li>
            <li>
            <li class="flex">
              <instagram-icon size="1x" class="custom-class"></instagram-icon>
              <a href="about-us.html">Instagram</a>
            </li>
          </ul>
        </div>
      </div>
      <hr style="border-color: white" />
      <div class="pb-12 text-center mt-12 text-xl">
        <p>
          © {{ new Date().getFullYear() }}
          <strong class="font-black">RightStay</strong>. All right reserved
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
