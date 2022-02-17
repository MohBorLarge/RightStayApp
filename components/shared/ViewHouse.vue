<template>
  <div class="pb-24">
    <div class="mb-12">
      <p class="text-5xl font-bold">{{ currentHouse.houseTitle }}</p>
      <p>{{ currentHouse.houseAddress }}, {{ currentHouse.state }}</p>
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
          <p>
            <span
              ><hard-drive-icon
                size="1.5x"
                class="custom-class mr-2"
              ></hard-drive-icon
            ></span>
            {{ currentHouse.noOfBedrooms }}
            bed(s)
          </p>
          <p>
            <span
              ><hard-drive-icon
                size="1.5x"
                class="custom-class mr-2"
              ></hard-drive-icon></span
            >{{ currentHouse.noOfBathrooms }} bath(s)
          </p>
          <p>
            <span
              ><square-icon
                size="1.3x"
                class="custom-class mr-2"
              ></square-icon></span
            >{{ currentHouse.squareFeet }} sqr feet
          </p>
        </div>
        <div class="grid grid-cols-3 gap-2 mb-8">
          <p
            v-for="(item, index) in currentHouse.houseFeatures"
            :key="index"
            class="bg-gray-200 rounded-lg px-2 py-1 w-full"
          >
            {{ item }}
          </p>
        </div>

        <div class="flex justify-between font-bold text-3xl">
          <p>Price per day</p>
          <p>₦{{ currentHouse.price }}</p>
        </div>
        <div>
          <form
            action="https://formsubmit.co/info@rightstay.ng"
            method="POST"
            class="grid grid-cols-1 gap-4 my-12"
          >
            <label for="fname">First name:</label>
            <input type="text" name="fname" placeholder="John" />
            <label for="lname">Last name:</label>
            <input type="text" name="lname" placeholder="Doe" />
            <label for="lname">Number of Days:</label>
            <input type="text" name="noOfDays" placeholder="4 Days" />
            <label for="email">Email:</label>
            <input type="email" name="email" placeholder="johndoe@mail.com" />
            <label for="phoneNumber">Phone Number:</label>
            <input type="number" name="phoneNumber" placeholder="080 1234 567" />
            <div class="flex justify-between">
              <div>
                <label for="noOfAdults">Adults:</label>
                <input type="number" name="noOfAdults" placeholder="2" />
              </div>
              <div>
                <label for="noOfKids">Children:</label>
                <input type="number" name="noOfKids" placeholder="2" />
              </div>
            </div>
            <label>From:</label>
            <input type="date" name="fromDate" />
            <label>To:</label>
            <input type="date" name="toDate" />

            <button
              class="bg-green-400 p-3 text-center rounded-md text-3xl text-white cursor-pointer"
              type="submit"
            >
              Book Now
            </button>
          </form>
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
        <div v-if="currentHouse.description" class="mb-12">
          <p
            v-for="(item, index) in currentHouse.description.content"
            :key="index"
            class="mb-6"
          >
            {{ item.content[0].value }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { HardDriveIcon, SquareIcon } from 'vue-feather-icons'

export default {
  name: 'ViewHouse',
  components: {
    HardDriveIcon,
    SquareIcon,
  },
  props: {
    currentHouse: {
      type: Object,
      default: () => {},
      required: true,
    },
  },
}
</script>

<style scoped>
form input {
  height: 40px;
  padding-left: 10px;
}
</style>
