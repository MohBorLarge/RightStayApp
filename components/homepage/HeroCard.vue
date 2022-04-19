<template>
  <vue-flux
    :options="options"
    :images="images"
    :transitions="transitions"
    class="anime rounded-lg"
  >
    <template #preloader>
      <flux-preloader />
    </template>
  </vue-flux>
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
      allowFullscreen: true,
      allowToSkipTransition: true,
      autohideTime: 2500,
      autoplay: true,
      bindKeys: false,
      delay: 5000,
      enableGestures: false,
      infinite: true,
      lazyLoad: true,
      lazyLoadAfter: 3,
    },
    images: [
      'https://images.ctfassets.net/y0slm2s1ky9o/61b7Yc2V6jdNxYHUkF0ORK/6d785d9a0f87adc0dfd15491272da047/newhome4.jpeg',
      'https://images.ctfassets.net/y0slm2s1ky9o/2jBntwmW1dh3xcH5m96eZh/022eb695a556002221fe92a3db496371/newhome7.jpeg',
      'https://images.ctfassets.net/y0slm2s1ky9o/4XFopUziaABw7OgMwBwCaB/c3f4088f1dcb07f1dfb7760ab9a47d89/home3.jpeg',
    ],
    transitions: [
      'blinds3d',
      'blocks2',
      'book',
      'cube',
      'round2',
      'swipe',
      'warp',
      'wave',
    ],
  }),
}
</script>
<style scoped>
.anime {
  height: 480px;
  background-image: linear-gradient(90deg,rgba(6,88,76,.9),rgba(255,0,0,0));
}
</style>
