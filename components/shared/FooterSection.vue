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
          <ul>
            <li><nuxt-link to="/all-houses">Short Lets</nuxt-link></li>
            <li><nuxt-link to="/about-rightstay">About RightStay</nuxt-link></li>
            <li><nuxt-link to="/privacy-policy">Privacy Policy</nuxt-link></li>
            <li><nuxt-link to="terms-conditions">Term &amp; Conditions</nuxt-link></li>
            <li><a href="shop.html">Rightsource Website</a></li>
          </ul>
        </div>
        <div class="w-1/4 text-xl">
          <ul>
            <li><a href="about-us.html">Twitter</a></li>
            <li><a href="contact-us.html">Facebook</a></li>
            <li><a href="careers.html">Instagram</a></li>
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
export default {
  name: 'FooterSection',
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
