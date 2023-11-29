<script setup lang="ts">
import { Carousel, initTE } from "tw-elements";
import { onMounted } from "vue";

onMounted(() => {
  initTE({ Carousel });
});
</script>

<template>
  <div class="relative">
    <!-- Hero Section -->
    <div class="grid grid-cols-3 items-center">
      <div class="col-span-2 pl-28">
        <div class="text-7xl font-extrabold font-['Raleway-Black']">
          <div class="pb-3">Healthy & Fresh</div>
          <div>Food For You</div>
        </div>
        <div class="text-xl py-6">
          Created for lovers of healthy, delicious, and <br />
          non-obvious food.
        </div>
        <a
          href="#menu"
          class="bg-orange-400 hover:bg-orange-300 rounded-lg py-2.5 px-4"
        >
          Check menu
          <svg
            class="inline mx-1"
            xmlns="http://www.w3.org/2000/svg"
            width="16"
            height="16"
            viewBox="0 0 16 16"
          >
            <path
              d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM8.5 4.5a.5.5 0 0 0-1 0v3h-3a.5.5 0 0 0 0 1h3v3a.5.5 0 0 0 1 0v-3h3a.5.5 0 0 0 0-1h-3v-3z"
            />
          </svg>
        </a>
      </div>
      <div class="col-span-1 relative bg-[#2E7D32] h-[92.5vh]">
        <div
          id="carouselExampleSlidesOnly"
          class="relative"
          data-te-carousel-init
          data-te-ride="carousel"
        >
          <!--Carousel items-->
          <div
            class="relative w-full inset-52 -left-96 overflow-hidden after:clear-both after:block after:content-['']"
          >
            <!--First item-->
            <div
              class="relative float-left -mr-[100%] w-full !transform-none opacity-0 transition-opacity duration-[600ms] ease-in-out motion-reduce:transition-none"
              data-te-carousel-fade
              data-te-carousel-item
              data-te-carousel-active
            >
              <img
                src="../assets/images/hero-section-slide-food-1.png"
                class="block w-full"
                alt="Kale Salad"
              />
            </div>
            <!--Second item-->
            <div
              class="relative float-left -mr-[100%] w-full !transform-none opacity-0 transition-opacity duration-[600ms] ease-in-out motion-reduce:transition-none"
              data-te-carousel-fade
              data-te-carousel-item
            >
              <img
                src="../assets/images/hero-section-slide-food-2.png"
                class="block w-full"
                alt="Tofu Southwestern"
              />
            </div>
            <!--Third item-->
            <div
              class="relative float-left -mr-[100%] w-full !transform-none opacity-0 transition-opacity duration-[600ms] ease-in-out motion-reduce:transition-none"
              data-te-carousel-fade
              data-te-carousel-item
            >
              <img
                src="../assets/images/hero-section-slide-food-3.png"
                class="block w-full"
                alt="Deconstructed Avacado"
              />
            </div>
            <!--Fourth item-->
            <div
              class="relative float-left -mr-[100%] w-full !transform-none opacity-0 transition-opacity duration-[600ms] ease-in-out motion-reduce:transition-none"
              data-te-carousel-fade
              data-te-carousel-item
            >
              <img
                src="../assets/images/hero-section-slide-food-4.png"
                class="block w-full"
                alt="Poke Bowl"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- Transition Break Image -->
    <div class="absolute">
      <img
        class="relative bottom-32 z-30"
        src="../assets/images/hero-section-food.png"
        alt=""
      />
    </div>
    <!-- About Us Section -->
    <div id="about-us" class="relative grid grid-cols-2 pt-32 items-center">
      <!-- About Us Food -->
      <div class="grid">
        <svg
          class="relative -left-56 col-start-1 row-start-1 z-0"
          width="625"
          height="625"
          viewBox="0 0 61 61"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <circle cx="30.5002" cy="30.5" r="30.5" fill="#2E7D32" />
        </svg>
        <img
          class="relative col-start-1 row-start-1 mt-24 ml-16 z-10"
          src="../assets/images/about-us-section-food.png"
          alt=""
        />
      </div>
      <!-- About Us Description -->
      <div class="flex flex-col gap-4 h-full items-left justify-center">
        <div class="text-orange-400 text-2xl">About Us</div>
        <div class="text-4xl font-semibold">Few words about us</div>
        <div class="text-2xl">
          <div>We are not ordinary food truck. We create a place</div>
          <div>overflowing with positive energy that it expresses</div>
          important to us values. Get to know them specifically.
          <div></div>
        </div>
      </div>
    </div>
    <!-- Menu Section -->
    <div id="menu" class="text-center py-32">
      <!-- Menu Heading -->
      <div class="mb-16">
        <div class="text-orange-400 text-2xl mb-3">Menu</div>
        <div class="text-4xl font-semibold">Explore our best food</div>
        <div class="text-xl mt-3">
          Below you can see our best selling meals!
        </div>
      </div>
      <!-- Menu Cards -->
      <div class="flex flex-col-3 my-10 mx-20 gap-6 justify-center">
        <!-- Card 1 -->
        <div class="shadow-2xl rounded-xl bg-gray-50 w-1/3">
          <img src="../assets/images/menu-section-mighty-burger.png" alt="" />
          <div class="my-5 ml-8 text-start">
            <div class="text-2xl font-semibold">Mighty Burger</div>
            <div class="mt-3">Served with fries and drink</div>
          </div>
        </div>
        <!-- Card 2 -->
        <div class="shadow-2xl rounded-xl bg-gray-50 w-1/3">
          <img src="../assets/images/menu-section-chickpae-salad.png" alt="" />
          <div class="my-5 ml-8 text-start">
            <div class="text-2xl font-semibold">Chickpae's salad</div>
            <div class="mt-3">Served with fries and drink</div>
          </div>
        </div>
        <!-- Card 3 -->
        <div class="shadow-2xl rounded-xl bg-gray-50 w-1/3">
          <img src="../assets/images/menu-section-chickpae-wrap.png" alt="" />
          <div class="my-5 ml-8 text-start">
            <div class="text-2xl font-semibold">Chickpae's wrap</div>
            <div class="mt-3">Served with fries and drink</div>
          </div>
        </div>
      </div>
    </div>
    <!-- Gallery Section -->
    <div class="pb-32 text-center">
      <div class="text-3xl font-semibold pb-10">Good food = happy clients</div>
      <div class="grid grid-cols-3 grid-rows-2">
        <img src="../assets//images/gallery-photo-1.png" alt="" />
        <img src="../assets//images/gallery-photo-2.png" alt="" />
        <img src="../assets//images/gallery-photo-3.png" alt="" />
        <img src="../assets//images/gallery-photo-4.png" alt="" />
        <img src="../assets//images/gallery-photo-5.png" alt="" />
        <img src="../assets//images/gallery-photo-6.png" alt="" />
      </div>
    </div>
    <!-- Contact Section -->
    <div id="contact" class="text-center pb-32">
      <!-- Menu Heading -->
      <div class="mb-16">
        <div class="text-orange-400 text-2xl mb-3">Contact</div>
        <div class="text-4xl font-semibold">We're waiting for you!</div>
      </div>
      <!-- Contact Cards -->
      <div class="flex flex-col-3 my-10 mx-96 gap-6 justify-center">
        <!-- Card 1 -->
        <div
          class="flex flex-col shadow-2xl rounded-full items-center bg-zinc-100 w-1/3"
        >
          <img class="h-10 mt-4" src="../assets/icons/time-icon.svg" alt="" />
          <div class="my-5 ml-8 text-center">
            <div class="text-2xl font-semibold">Today 12 pm - 9 pm</div>
            <div class="mt-3">Working Hours</div>
          </div>
        </div>
        <!-- Card 2 -->
        <div
          class="flex flex-col shadow-2xl rounded-full items-center bg-zinc-100 w-1/3"
        >
          <img class="h-10 mt-4" src="../assets/icons/map-icon.svg" alt="" />
          <div class="my-5 ml-8 text-center">
            <div class="text-2xl font-semibold">3883 Rupert St. Vancouver</div>
            <div class="mt-3">Find Us</div>
          </div>
        </div>
        <!-- Card 3 -->
        <div
          class="flex flex-col shadow-2xl rounded-full items-center bg-zinc-100 w-1/3"
        >
          <img class="h-10 mt-4" src="../assets/icons/phone-icon.svg" alt="" />
          <div class="my-5 ml-8 text-center">
            <div class="text-2xl font-semibold">(604) 569-2198</div>
            <div class="mt-3">Call to Us</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
