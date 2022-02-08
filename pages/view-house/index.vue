<template>
  <div>
    <div>
      <p>Lekki Gardens</p>
      <p>4.8/5 (34532 reviews) # Lekki, Lagos</p>
    </div>
    <div class="flex w-full my-10">
      <div class="images w-full mr-10">
        <div class="flex mb-10">
          <div class="mr-6 w-full">
            <img
              src="@/assets/images/girl.jpg"
              alt=""
              srcset=""
              class="h-full rounded-md"
            />
          </div>
          <div class="w-3/12 grid grid-cols-1 gap-6">
            <div
              v-for="item in [1, 2, 3, 4]"
              :key="item"
              class=""
            >
              <img src="@/assets/images/girl.jpg" alt="" srcset="" class="rounded-md"/>
            </div>
          </div>
        </div>
        <div class="flex justify-between mr-96">
          <p>Description</p>
          <p>Room and facilities</p>
          <p>Testimonials</p>
        </div>
      </div>
      <div class="facilities w-4/12">
        <p class="text-4xl font-bold mb-8">Facilities</p>
        <div class="flex justify-between w-8/12 mb-6">
          <p>3 bed</p>
          <p>4 bath</p>
          <p>55 sqr feet</p>
        </div>
        <div class="grid grid-cols-3 gap-2">
          <p class="bg-blue-200 rounded p-1 w-24">Guest Toilet</p>
          <p class="bg-blue-200 rounded p-1 w-24">Guest Toilet</p>
          <p class="bg-blue-200 rounded p-1 w-24">Guest Toilet</p>
          <p class="bg-blue-200 rounded p-1 w-24">Guest Toilet</p>
          <p class="bg-blue-200 rounded p-1 w-24">Guest Toilet</p>
          
        </div>
        <div class="my-8">
          <div class="flex justify-between text-xl mb-4">
            <p class="font-bold">Property Type</p>
            <p>Apartment</p>
          </div>
          <div class="flex justify-between text-xl mb-4">
            <p class="font-bold">Check In</p>
            <p>01/01/2022</p>
          </div>
          <div class="flex justify-between text-xl mb-4">
            <div>
              <p class="font-bold">Duration</p>
              <p class="text-sm">@ $1500</p>
            </div>
            <div>
              <p class="font-bold">3 Days</p>
              <p class="text-sm">$4500</p>
            </div>
          </div>
          <div class="flex justify-between text-xl">
            <p class="font-bold">Sales Tax</p>
            <p>$10</p>
          </div>
        </div>
        <div>
          <div class="flex justify-between font-extrabold text-3xl mb-4">
            <p class="">Total</p>
            <p>$4510</p>
          </div>
          <div class="bg-green-400 p-3 text-center rounded-md text-3xl text-white">
            <button>Rent Now</button>
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ViewHouse',
  layout: 'DefaultLayout',
}
</script>
