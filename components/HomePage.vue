<template>
<div>
  <div class="container">
    <HeaderBar />
    <HeroCard />
    <div class="mt-20 mb-24">
      <p class="w-64 text-2xl">We are already all around Lagos.</p>
    </div>
    <div class="text-center text-2xl my-12 mx-auto">
      <a href="#" class="text-green-400 hover:text-green-700"
        >View All Houses</a
      >
    </div>
    <HouseView />
  </div>
  <FooterSection />
</div>  
</template>

<script>


export default {
  name: 'HomePage',
  
  data() {
    return {}
  },
}
</script>
