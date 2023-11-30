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
      <!-- Hero Content -->
      <div class="col-span-2 pl-28">
        <div class="font-['Raleway-Black'] text-7xl font-extrabold">
          <div class="pb-3">Healthy & Fresh</div>
          <div>Food For You</div>
        </div>
        <div class="py-6 text-xl">
          Created for lovers of healthy, delicious, and <br />
          non-obvious food.
        </div>
        <a
          href="#menu"
          class="rounded-lg bg-orange-400 px-4 py-2.5 hover:bg-orange-300"
        >
          Check menu
          <svg
            class="mx-1 inline"
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
      <!-- Hero Carousel -->
      <div class="relative col-span-1 h-[92.5vh] bg-[#2E7D32]">
        <div
          id="carouselExampleSlidesOnly"
          class="relative"
          data-te-carousel-init
          data-te-ride="carousel"
        >
          <!--Carousel items-->
          <div
            class="relative inset-52 -left-96 w-full overflow-hidden duration-700 after:clear-both after:block after:content-[''] hover:scale-105 hover:brightness-110"
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
        class="relative bottom-32 z-30 duration-700 hover:scale-110 hover:brightness-125"
        src="../assets/images/hero-section-food.png"
        alt=""
      />
    </div>
    <!-- About Us Section -->
    <div id="about-us" class="relative grid grid-cols-2 items-center pt-32">
      <!-- About Us Food -->
      <div class="grid">
        <svg
          class="relative -left-56 z-0 col-start-1 row-start-1"
          width="625"
          height="625"
          viewBox="0 0 61 61"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <circle cx="30.5002" cy="30.5" r="30.5" fill="#2E7D32" />
        </svg>
        <img
          class="relative z-10 col-start-1 row-start-1 ml-16 mt-24 duration-700 hover:scale-105 hover:brightness-110"
          src="../assets/images/about-us-section-food.png"
          alt=""
        />
      </div>
      <!-- About Us Description -->
      <div class="items-left flex h-full flex-col justify-center gap-4">
        <div class="text-2xl text-orange-400">About Us</div>
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
    <div id="menu" class="py-32 text-center">
      <!-- Menu Heading -->
      <div class="mb-16">
        <div class="mb-3 text-2xl text-orange-400">Menu</div>
        <div class="text-4xl font-semibold">Explore our best food</div>
        <div class="mt-3 text-xl">
          Below you can see our best selling meals!
        </div>
      </div>
      <!-- Menu Cards -->
      <div class="flex-col-3 mx-20 my-10 flex justify-center gap-6">
        <!-- Card 1 -->
        <div
          class="w-1/3 rounded-xl bg-gray-50 shadow-2xl duration-700 hover:scale-105 hover:brightness-125"
        >
          <img src="../assets/images/menu-section-mighty-burger.png" alt="" />
          <div class="my-5 ml-8 text-start">
            <div class="text-2xl font-semibold">Mighty Burger</div>
            <div class="mt-3">Served with fries and drink</div>
          </div>
        </div>
        <!-- Card 2 -->
        <div
          class="w-1/3 rounded-xl bg-gray-50 shadow-2xl duration-700 hover:scale-105 hover:brightness-125"
        >
          <img src="../assets/images/menu-section-chickpae-salad.png" alt="" />
          <div class="my-5 ml-8 text-start">
            <div class="text-2xl font-semibold">Chickpae's salad</div>
            <div class="mt-3">Served with fries and drink</div>
          </div>
        </div>
        <!-- Card 3 -->
        <div
          class="w-1/3 rounded-xl bg-gray-50 shadow-2xl duration-700 hover:scale-105 hover:brightness-125"
        >
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
      <div class="pb-10 text-3xl font-semibold">Good food = happy clients</div>
      <div class="grid grid-cols-3 grid-rows-2">
        <img
          class="duration-700 hover:scale-105 hover:brightness-125"
          src="../assets//images/gallery-photo-1.png"
          alt=""
        />
        <img
          class="duration-700 hover:scale-105 hover:brightness-125"
          src="../assets//images/gallery-photo-2.png"
          alt=""
        />
        <img
          class="duration-700 hover:scale-105 hover:brightness-125"
          src="../assets//images/gallery-photo-3.png"
          alt=""
        />
        <img
          class="duration-700 hover:scale-105 hover:brightness-125"
          src="../assets//images/gallery-photo-4.png"
          alt=""
        />
        <img
          class="duration-700 hover:scale-105 hover:brightness-125"
          src="../assets//images/gallery-photo-5.png"
          alt=""
        />
        <img
          class="duration-700 hover:scale-105 hover:brightness-125"
          src="../assets//images/gallery-photo-6.png"
          alt=""
        />
      </div>
    </div>
    <!-- Contact Section -->
    <div id="contact" class="pb-32 text-center">
      <!-- Menu Heading -->
      <div class="mb-16">
        <div class="mb-3 text-2xl text-orange-400">Contact</div>
        <div class="text-4xl font-semibold">We're waiting for you!</div>
      </div>
      <!-- Contact Cards -->
      <div class="flex-col-3 mx-96 my-10 flex justify-center gap-6">
        <!-- Card 1 -->
        <div
          class="flex w-1/3 flex-col items-center rounded-full bg-zinc-100 shadow-2xl"
        >
          <img class="mt-4 h-10" src="../assets/icons/time-icon.svg" alt="" />
          <div class="my-5 ml-8 text-center">
            <div class="text-2xl font-semibold">Today 12 pm - 9 pm</div>
            <div class="mt-3">Working Hours</div>
          </div>
        </div>
        <!-- Card 2 -->
        <div
          class="flex w-1/3 flex-col items-center rounded-full bg-zinc-100 shadow-2xl"
        >
          <img class="mt-4 h-10" src="../assets/icons/map-icon.svg" alt="" />
          <div class="my-5 ml-8 text-center">
            <div class="text-2xl font-semibold">3883 Rupert St. Vancouver</div>
            <div class="mt-3">Find Us</div>
          </div>
        </div>
        <!-- Card 3 -->
        <div
          class="flex w-1/3 flex-col items-center rounded-full bg-zinc-100 shadow-2xl"
        >
          <img class="mt-4 h-10" src="../assets/icons/phone-icon.svg" alt="" />
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
