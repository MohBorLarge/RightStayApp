<template>
<div class="px-24">
  <header class="flex my-12 justify-between">
    <img src="@/assets/RightStayLogo/svg/bluegreen.svg" alt="" class="w-40">
    <div class="flex">
      <a href="#" class="pr-4">Home Type</a>
      <a href="#" class="pr-4">About Us</a>
      <a href="#" class="pr-4">Contact</a>
      <a href="#" class="pr-4">Blog</a>
      <a href="#">Buy Property</a>
    </div>
  </header>
  <div class="hero pl-16 pt-20 ">
    <p class="text-3xl text-white w-56 mb-6">Find the perfect place to stay with your family</p>
    <div class="text-sm text-white mb-6">
      <p>Family is number one and comfort is number two.</p>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
    </div>
    <div class="card w-96 h-16 p-2 flex justify-between">
      <div>
        <p>location</p>
        <p class="text-green-400">London</p>
      </div>
      <div>
        <p>Type</p>
        <p class="text-green-400">Duplex</p>
      </div>
      <div>
        <p>Maximum Price</p>
        <p class="text-green-400">$5000</p>
      </div>
      <div>
        <button class="w-20 h-10 bg-green-400 text-white">Search</button>
      </div>

    </div>
  </div>
  <div class="mt-16">
      <p>We are all around Lagos</p>
    </div>
  
</div>
    
</template>

<script>
export default {
  name: 'HomePage',
}
</script>

<style scoped>
.hero {
  background-image: url('@/assets/images/home1.jpg'); 
  background-repeat: no-repeat;
  background-size: cover;
  width: 100%;
  height: 450px;
 }
 .card {
   background-color: white;
 }
</style>