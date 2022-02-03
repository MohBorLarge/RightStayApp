<template>
  <div class="px-24">
    <header class="flex my-12 justify-between">
      <img src="@/assets/RightStayLogo/svg/bluegreen.svg" alt="" class="w-40" />
      <div class="flex text-green-400">
        <a href="#" class="hover:text-green-700 pr-4 font-semibold"
          >Home Type</a
        >
        <a href="#" class="hover:text-green-700 pr-4 font-semibold">About Us</a>
        <a href="#" class="hover:text-green-700 pr-4 font-semibold">Contact</a>
        <a href="#" class="hover:text-green-700 pr-4 font-semibold">Blog</a>
        <a href="#" class="hover:text-green-700 font-semibold">Buy Property</a>
      </div>
    </header>
    <div class="hero pl-16 pt-20 w-full bg-cover bg-no-repeat">
      <p class="text-3xl text-white w-56 mb-6">
        Find the perfect place to stay with your family
      </p>
      <div class="text-sm text-white mb-6">
        <p>Family is number one and comfort is number two.</p>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
      </div>
      <div class="bg-white w-2/5 h-20 p-4 flex justify-between">
        <form class="text-sm">
          <label class="block">Location</label>
          <input
            type="text"
            name=""
            value="London"
            class="text-green-400 w-14 border-none border-transparent"
          />
        </form>
        <form class="text-sm">
          <label class="block">Type</label>
          <input
            type="text"
            name=""
            value="Duplex"
            class="text-green-400 w-14 border-none"
          />
        </form>
        <form class="text-sm">
          <label class="block">Maximum Price</label>
          <input
            type="text"
            name=""
            value="$5000"
            class="text-green-400 w-14 order-none"
          />
        </form>
        <div>
          <button
            class="w-24 h-10 bg-green-600 hover:bg-green-700 text-white rounded"
          >
            Search
          </button>
        </div>
      </div>
    </div>
    <div class="mt-20 mb-24">
      <p class="w-64 text-2xl">We are already all around Lagos.</p>
    </div>
    <div class="text-center text-2xl my-12 mx-auto">
      <a href="#" class="text-green-400 hover:text-green-700"
        >View All Houses</a
      >
    </div>
    <div class="flex">
      <p class="text-green-400 w-3/6 mt-8 mr-24 text-xl">Lagos State</p>
      <div class="grid grid-cols-3 gap-10 mb-12">
        <div
          v-for="item in [1, 2, 3, 4, 5, 6, 7, 8, 9]"
          :key="item"
          class="bg-white p-4 rounded-lg"
        >
          <div class="pb-6">
            <img src="@/assets/images/home3.jpeg" alt="" class="rounded-lg" />
          </div>
          <div class="text-xl mb-2">
            <p class="text-green-400">$300,000</p>
          </div>
          <div class="location flex text-gray-400">
            <div>
              <LocationSharp
                class="text-gray-400 h-4"
                style="margin: 3px 2px 0 0"
              />
            </div>
            <p>Preston Rd, Birmingham</p>
          </div>
          <div class="details flex justify-between">
            <div class="flex text-gray-400">
              <BedOutline class="h-4" style="margin: 3px 3px 0 0" />
              <p>4 Bd.</p>
            </div>
            <div class="flex text-gray-400">
              <SBath class="h-4" style="margin: 3px 3px 0 0" />
              <p>2 Ba.</p>
            </div>
            <div class="flex text-gray-400">
              <SquareSharp class="h-4" style="margin: 3px 3px 0 0" />
              <p>890 sqft.</p>
            </div>
          </div>
          <div
            class="bg-green-600 hover:bg-green-700 text-white py-2 w-full mt-4 text-center rounded-md"
          >
            <button>View House</button>
          </div>
        </div>
      </div>
    </div>
    <!-- <div>
      <div class="grid grid-cols-4 gap-12 bg-white text-green-400 py-12 pl-16">
        <div class="about-us">
          <p>About Us</p>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Consequatur, id temporibus? Voluptate neque dolore maiores ut modi
            dolorum libero assumenda accusantium ratione natus nulla tempora ex
            molestias, illum reiciendis incidunt?
          </p>
          <p>fb</p>
        </div>
        <div class="get-in-touch">
          <p>loc: 123 Street, Lagos, Nigeria</p>
          <p>call: +234 12345678</p>
          <p>mail: info@example.com</p>
          <p>time: Mon - Fri, 9am - 5pm</p>
        </div>
        <div class="useful-link">
          <p>Useful Link</p>
          <div>
            <div><a href="#">lorem</a></div>
            <div><a href="#">lorem</a></div>
            <div><a href="#">lorem</a></div>
            <div><a href="#">lorem</a></div>
          </div>
        </div>
        <div class="parent-company">
          <a href="#">RightSource.com</a>
        </div>
      </div>
    </div> -->
  </div>
</template>

<script>
import { BedOutline, LocationSharp, SquareSharp } from 'vue-icon-packs/io'
import { SBath } from 'vue-icon-packs/bx'

export default {
  name: 'HomePage',
  components: { BedOutline, LocationSharp, SBath, SquareSharp },
}
</script>
