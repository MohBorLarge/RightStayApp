<template>
  <div class="pb-24">
    <div class="mb-12">
      <p class="text-5xl font-bold">Lekki Gardens</p>
      <p>Preston Rd, Birmingham, Lekki, Lagos</p>
    </div>
    <div class="flex w-full">
      <div class="images w-full mr-10">
        <div class="flex mb-10">
          <div class="mr-6 w-full">
            <img
              src="@/assets/images/newhome1.jpeg"
              alt=""
              srcset=""
              class="h-full rounded-md"
            />
          </div>
          <div class="w-3/12 grid grid-cols-1 gap-6">
            <div v-for="item in [1, 2, 3, 4]" :key="item" class="">
              <img
                src="@/assets/images/newhome3.jpeg"
                alt=""
                srcset=""
                class="rounded-md object-cover"
              />
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="grid grid-cols-2 gap-16">
      <div>
        <p class="text-4xl font-bold mb-8">Facilities</p>
        <div class="flex justify-between w-8/12 mb-6">
          <p>3 bed</p>
          <p>4 bath</p>
          <p>55 sqr feet</p>
        </div>
        <div class="grid grid-cols-3 gap-2">
          <p class="bg-gray-200 rounded-lg px-2 py-1 w-full">Guest Toilet</p>
          <p class="bg-gray-200 rounded-lg px-2 py-1 w-full">Kitchen</p>
          <p class="bg-gray-200 rounded-lg px-2 py-1 w-full">Guest Toilet</p>
          <p class="bg-gray-200 rounded-lg px-2 py-1 w-full">Guest Toilet</p>
          <p class="bg-gray-200 rounded-lg px-2 py-1 w-full">Guest Toilet</p>
        </div>
        <div>
          <div class="flex justify-between font-bold text-3xl mb-4">
            <p class="">Total</p>
            <p>$4510</p>
          </div>
          <div
            class="bg-green-400 p-3 text-center rounded-md text-3xl text-white cursor-pointer"
          >
            Rent Now
          </div>
        </div>
      </div>

      <div>
        <div
          class="flex justify-between mr-96 cursor-pointer mb-8 text-xl font-semibold"
        >
          <div>
            <p class="ease">Description</p>
            <hr class="text-green-400 mt-2" style="border-top: 2px solid" />
          </div>
        </div>
        <div class="mb-12">
          <p>
            We may be biased but Lekki Gardens Apartment is one of the coolest
            place around. The apartment covers 65m and comes with a separate
            apartment for any extended guests to enjoy their privacy. There is a
            master bedroom with its own terrace, two double bedrooms and a
            wellness space comprising a Jacuzzi, hammam,sauna and pool <br />
            Arrive through the front or through the side gate, which spectuarly
            opens to a garrage -- but dont be mistaken, this is no normal
            garrage. This magnificent museum-like room can fit up to one car.
            Together this property is equally as perfect for group getaways as
            it is for corporate events such as product launches
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ViewHouse',
}
</script>
