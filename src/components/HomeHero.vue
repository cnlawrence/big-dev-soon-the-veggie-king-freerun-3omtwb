<script setup lang="ts">
import { Carousel, initTE } from "tw-elements";
import { onMounted } from "vue";

onMounted(() => {
  initTE({ Carousel });
});
</script>

<template>
  <div class="grid grid-flow-row">
    <!-- Hero Section -->
    <div class="relative flex flex-row pl-4 md:pl-10 lg:items-center lg:pl-20">
      <!-- Hero Content -->
      <div class="basis-auto pr-8 pt-32 sm:basis-10/12 sm:px-2 sm:pr-0 lg:pt-0">
        <div
          class="font-['Raleway-Black'] text-3xl font-extrabold sm:text-6xl lg:text-7xl"
        >
          <div class="pb-3">Healthy & Fresh</div>
          <div>Food For You</div>
        </div>
        <div class="w-3/4 py-6 sm:text-xl">
          Created for lovers of healthy, delicious, and non-obvious food.
        </div>
        <a
          href="#menu"
          class="inline-flex gap-2 rounded-lg bg-orange-400 px-5 py-2.5 hover:bg-orange-300"
        >
          <div>Check menu</div>
          <img class="w-5" src="../assets/icons/check-menu-icon.svg" alt="" />
        </a>
      </div>
      <!-- Hero Carousel -->
      <div
        class="relative h-[67vh] w-full basis-3/12 bg-[#2E7D32] sm:basis-5/12 lg:h-[85vh] lg:basis-3/12"
      >
        <div
          id="carouselExampleSlidesOnly"
          class="absolute inset-0 right-0 w-[40vh] -translate-x-[25%] translate-y-[10%] sm:w-[60vh] sm:-translate-x-[17%] lg:-translate-x-[65%]"
          data-te-carousel-init
          data-te-ride="carousel"
        >
          <!--Carousel items-->
          <div
            class="relative overflow-hidden duration-700 after:clear-both after:block after:content-[''] hover:scale-105 hover:brightness-110"
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
      <!-- Transition Break Image -->
      <div class="absolute bottom-0 left-0 basis-0 translate-y-[50%]">
        <img
          class="z-30 duration-700 hover:scale-110 hover:brightness-125"
          src="../assets/images/hero-section-food.png"
          alt=""
        />
      </div>
    </div>

    <!-- About Us Section -->
    <div id="about-us" class="relative my-32 flex items-center">
      <!-- About Us Food -->
      <div class="min-h-full md:basis-[47%]">
        <svg
          class="absolute right-0 z-0 min-w-[550px] max-w-[35%] translate-x-[80%] translate-y-[30%] md:left-0 md:-translate-x-[60%] md:-translate-y-0 xl:-translate-x-[40%]"
          viewBox="0 0 61 61"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <circle cx="30.5002" cy="30.5" r="30.5" fill="#2E7D32" />
        </svg>
        <img
          class="absolute right-0 z-10 min-w-[300px] max-w-[25%] translate-x-[40%] translate-y-[100%] duration-700 hover:scale-105 hover:brightness-110 md:left-0 md:min-w-[375px] md:-translate-x-[23%] md:translate-y-[25%] xl:translate-x-[18%]"
          src="../assets/images/about-us-section-food.png"
          alt=""
        />
      </div>
      <!-- About Us Description -->
      <div class="items-left mx-4 my-[10%] h-full justify-center gap-4">
        <div class="py-2 text-xl text-orange-400 sm:text-2xl">About Us</div>
        <div class="py-2 text-2xl font-semibold sm:text-4xl">
          Few words about us
        </div>
        <div class="py-2 text-lg sm:text-2xl">
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
        <div class="mb-3 text-lg text-orange-400 sm:text-2xl">Menu</div>
        <div class="text-xl font-semibold sm:text-4xl">
          Explore our best food
        </div>
        <div class="mt-3 sm:text-xl">
          Below you can see our best selling meals!
        </div>
      </div>
      <!-- Menu Cards -->
      <div
        class="mx-auto my-10 grid grid-cols-1 justify-center gap-6 sm:mx-10 md:grid-cols-3 md:gap-3 lg:mx-20"
      >
        <!-- Card 1 -->
        <div
          class="mx-2 rounded-2xl bg-gray-50 shadow-2xl duration-700 hover:scale-105 hover:brightness-125"
        >
          <img src="../assets/images/menu-section-mighty-burger.png" alt="" />
          <div class="mx-4 my-5 text-start">
            <div class="text-xl font-semibold sm:text-2xl">Mighty Burger</div>
            <div class="mt-3">Served with fries and drink</div>
          </div>
        </div>
        <!-- Card 2 -->
        <div
          class="mx-2 rounded-2xl bg-gray-50 shadow-2xl duration-700 hover:scale-105 hover:brightness-125"
        >
          <img src="../assets/images/menu-section-chickpae-salad.png" alt="" />
          <div class="mx-4 my-5 text-start">
            <div class="text-xl font-semibold sm:text-2xl">
              Chickpae's salad
            </div>
            <div class="mt-3">Served with fries and drink</div>
          </div>
        </div>
        <!-- Card 3 -->
        <div
          class="mx-2 rounded-2xl bg-gray-50 shadow-2xl duration-700 hover:scale-105 hover:brightness-125"
        >
          <img src="../assets/images/menu-section-chickpae-wrap.png" alt="" />
          <div class="mx-4 my-5 text-start">
            <div class="text-xl font-semibold sm:text-2xl">Chickpae's wrap</div>
            <div class="mt-3">Served with fries and drink</div>
          </div>
        </div>
      </div>
    </div>
    <!-- Gallery Section -->
    <div class="pb-32 text-center">
      <div class="pb-10 text-xl font-semibold sm:text-3xl">
        Good food = happy clients
      </div>
      <div class="grid grid-rows-2 sm:grid-cols-3">
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
    <div id="contact" class="mx-auto bg-white px-1 pb-48 pt-16 sm:px-6 lg:px-8">
      <!-- Menu Heading -->
      <div class="mb-16 text-center">
        <div
          class="mb-3 text-lg text-orange-400 sm:text-2xl sm:leading-tight sm:tracking-tight"
        >
          Contact Us
        </div>
        <div class="mt-4 text-xl font-semibold sm:text-4xl">
          We're waiting for you!
        </div>
      </div>
      <!-- Contact Cards -->
      <div
        class="mx-auto grid gap-8 sm:px-6 lg:grid-cols-2 lg:px-8 xl:grid-cols-3"
      >
        <!-- Card 1 -->
        <div class="rounded-full border bg-zinc-100 shadow-2xl">
          <img
            class="mx-auto mt-4 h-10"
            src="../assets/icons/time-icon.svg"
            alt=""
          />
          <div class="mx-4 my-5 text-center">
            <div class="text-xl font-semibold sm:text-2xl">
              Today 12 pm - 9 pm
            </div>
            <div class="mt-3">Working Hours</div>
          </div>
        </div>
        <!-- Card 2 -->
        <div class="rounded-full border bg-zinc-100 shadow-2xl">
          <img
            class="mx-auto mt-4 h-10"
            src="../assets/icons/map-icon.svg"
            alt=""
          />
          <div class="mx-4 my-5 text-center">
            <div class="text-xl font-semibold sm:text-2xl">
              3883 Rupert St. Vancouver
            </div>
            <div class="mt-3">Find Us</div>
          </div>
        </div>
        <!-- Card 3 -->
        <div
          class="rounded-full border bg-zinc-100 shadow-2xl md:col-span-2 md:mx-auto md:w-1/2 xl:col-span-1 xl:mx-0 xl:w-full"
        >
          <img
            class="mx-auto mt-4 h-10"
            src="../assets/icons/phone-icon.svg"
            alt=""
          />
          <div class="mx-4 my-5 text-center">
            <div class="text-xl font-semibold sm:text-2xl">(604) 569-2198</div>
            <div class="mt-3">Call to Us</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
