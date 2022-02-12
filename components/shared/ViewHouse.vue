<template>
  <div>
    <div>
      <p class="text-5xl font-bold tracking-widest">Lekki Gardens</p>
      <p>4.8/5 (34532 reviews) # Lekki, Lagos</p>
    </div>
    <div class="flex w-full my-8">
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
        <div
          class="flex justify-between mr-96 cursor-pointer mb-8 text-xl font-semibold"
        >
          <div>
            <p class="ease" @click="switchTab('1')">Description</p>
            <hr v-show="hidden1" class="text-green-400" />
          </div>
          <div>
            <p class="ease" @click="switchTab('2')">Room and facilities</p>
            <hr v-show="hidden2" class="text-green-400" />
          </div>
          <div>
            <p class="ease" @click="switchTab('3')">Testimonials</p>
            <hr v-show="hidden3" class="text-green-400" />
          </div>
        </div>
        <div class="mb-12">
          <div v-show="hidden1">
            <p>
              We may be biased but Lekki Gardens Apartment is one of the coolest
              place around. The apartment covers 65m and comes with a separate
              apartment for any extended guests to enjoy their privacy. There is
              a master bedroom with its own terrace, two double bedrooms and a
              wellness space comprising a Jacuzzi, hammam,sauna and pool <br />
              Arrive through the front or through the side gate, which
              spectuarly opens to a garrage -- but dont be mistaken, this is no
              normal garrage. This magnificent museum-like room can fit up to
              one car. Together this property is equally as perfect for group
              getaways as it is for corporate events such as product launches
            </p>
          </div>

          <p v-show="hidden2">hffekhqhkdwhh 2222222</p>
          <p v-show="hidden3">dhjsbjhds 3333333</p>
        </div>
      </div>
      <div class="facilities w-4/12">
        <p class="text-4xl font-bold mb-8 tracking-widest">Facilities</p>
        <div class="flex justify-between w-8/12 mb-6">
          <p>3 bed</p>
          <p>4 bath</p>
          <p>55 sqr feet</p>
        </div>
        <div class="grid grid-cols-3 gap-2">
          <p class="bg-gray-200 rounded p-1 w-24">Guest Toilet</p>
          <p class="bg-gray-200 rounded p-1 w-24">Kitchen</p>
          <p class="bg-gray-200 rounded p-1 w-24">Guest Toilet</p>
          <p class="bg-gray-200 rounded p-1 w-24">Guest Toilet</p>
          <p class="bg-gray-200 rounded p-1 w-24">Guest Toilet</p>
        </div>
        <div class="my-8">
          <div class="flex justify-between text-xl mb-4">
            <p class="font-semibold">Property Type</p>
            <p>Apartment</p>
          </div>
          <div class="flex justify-between text-xl mb-4">
            <p class="font-semibold">Check In</p>
            <p>01/01/2022</p>
          </div>
          <div class="flex justify-between text-xl mb-4">
            <div>
              <p class="font-semibold">Duration</p>
              <p class="text-sm">@ $1500</p>
            </div>
            <div>
              <p class="font-semibold">3 Days</p>
              <p class="text-sm">$4500</p>
            </div>
          </div>
          <div class="flex justify-between text-xl">
            <p class="font-semibold">Sales Tax</p>
            <p>$10</p>
          </div>
        </div>
        <div>
          <div class="flex justify-between font-bold text-3xl mb-4">
            <p class="">Total</p>
            <p>$4510</p>
          </div>
          <div
            class="bg-green-400 p-3 text-center rounded-md text-3xl text-white"
          >
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
  data() {
    return {
      hidden1: true,
      hidden2: false,
      hidden3: false,
    }
  },
  methods: {
    switchTab(tab) {
      if (tab === '1') {
        this.hidden1 = true
        this.hidden2 = false
        this.hidden3 = false
      } else if (tab === '2') {
        this.hidden1 = false
        this.hidden2 = true
        this.hidden3 = false
      } else {
        this.hidden1 = false
        this.hidden2 = false
        this.hidden3 = true
      }
    },
  },
}
</script>


