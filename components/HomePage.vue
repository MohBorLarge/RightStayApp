<template>
<div class="px-24">
  <header class="flex my-12 justify-between">
    <img src="@/assets/RightStayLogo/svg/bluegreen.svg" alt="" class="w-40">
    <div class="flex">
      <a href="#" class="hover:text-green-400 pr-4 font-semibold">Home Type</a>
      <a href="#" class="hover:text-green-400 pr-4 font-semibold">About Us</a>
      <a href="#" class="hover:text-green-400 pr-4 font-semibold">Contact</a>
      <a href="#" class="hover:text-green-400 pr-4 font-semibold">Blog</a>
      <a href="#" class="hover:text-green-400 font-semibold">Buy Property</a>
    </div>
  </header>
  <div class="hero pl-16 pt-20 w-full bg-cover bg-no-repeat">
    <p class="text-3xl text-white w-56 mb-6">Find the perfect place to stay with your family</p>
    <div class="text-sm text-white mb-6">
      <p>Family is number one and comfort is number two.</p>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
    </div>
    <div class="bg-white w-2/5 h-20 p-4 flex justify-between">
      <form class="text-sm">
        <label>Location</label>
        <input type="text" name="" value="London" class="text-green-400 w-14 border-none border-transparent">
      </form>
      <form class="text-sm">
        <label>Type</label>
        <input type="text" name="" value="Duplex" class="text-green-400 w-14 border-none">
      </form>
      <form class="text-sm">
        <label>Maximum Price</label>
        <input type="text" name="" value="$5000" class="text-green-400 w-14 order-none">
      </form>
      <div>
        <button class="w-24 h-10 bg-green-400 text-white">Search</button>
      </div>

    </div>
  </div>
  <div class="mt-20 mb-24">
    <p class="w-64 text-2xl">We are already all around Lagos.</p>
  </div>
  <div class="flex">
    <p class="text-green-400 w-3/6 mt-8 mr-24 text-xl">Lagos State</p>
    <div class="grid grid-cols-3 gap-7">
      <div class="">
        <img src="@/assets/images/home3.jpeg" alt="">
      </div>
      <div class="">
        <img src="@/assets/images/home2.jpg" alt="">
      </div>
      <div class="">
        <img src="@/assets/images/home3.jpeg" alt="">
      </div>
    </div>
  </div>

  
</div>    
</template>

<script>
export default {
  name: 'HomePage',
}
</script>