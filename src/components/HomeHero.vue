<script setup lang="ts">
import { Carousel, initTE } from "tw-elements";
import { onMounted } from "vue";

onMounted(() => {
  initTE({ Carousel });
});
</script>

<template>
  <div class="relative">
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
        <button
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
        </button>
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
    <div class="absolute">
    <img
        class="relative bottom-32 z-30"
      src="../assets/images/hero-section-food.png"
      alt=""
    />
  </div>
</template>

<style scoped></style>
