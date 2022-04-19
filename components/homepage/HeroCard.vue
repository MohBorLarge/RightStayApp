<template>
  <div class="relative">
    <vue-flux
      :options="options"
      :images="images"
      :transitions="transitions"
      class="custom"
    >
      <template #preloader>
        <flux-preloader />
      </template>
    </vue-flux>

    <div class="hero bg-cover">
      <div class="hero-overlay">
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
import { VueFlux, FluxPreloader } from 'vue-flux'
export default {
  name: 'HeroCard',
  components: {
    VueFlux,
    FluxPreloader,
  },
  props: {
    text: {
      type: String,
      default: '',
      required: true,
    },
  },
  data: () => ({
    options: {
      allowFullscreen: false,
      allowToSkipTransition: true,
      autohideTime: 2500,
      autoplay: true,
      bindKeys: false,
      delay: 2000,
      enableGestures: false,
      infinite: true,
      lazyLoad: true,
      lazyLoadAfter: 3,
    },
    images: [
      'https://images.ctfassets.net/y0slm2s1ky9o/61b7Yc2V6jdNxYHUkF0ORK/6d785d9a0f87adc0dfd15491272da047/newhome4.jpeg',
      'https://images.ctfassets.net/y0slm2s1ky9o/PqzgoHkzJVIWEWPOURYil/5ad16a352fd230bc55870f442840e4fc/Unknown1.jpeg',
      'https://images.ctfassets.net/y0slm2s1ky9o/2jBntwmW1dh3xcH5m96eZh/022eb695a556002221fe92a3db496371/newhome7.jpeg',
    ],
    transitions: [
      'fade',
      'kenburn',
      'blocks2',
      'waterfall',
      'blinds2d',
      'blocks1',
      'cube',
      'explode'
    ],
  }),
}
</script>
<style scoped>
.custom {
  height: 480px;
}
</style>
