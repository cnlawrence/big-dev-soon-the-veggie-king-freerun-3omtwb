<script setup lang="ts"></script>

<template>
  <div class="relative">
    <div class="grid grid-cols-3 items-center">
      <div class="col-span-2 pl-28">
        <div class="text-7xl font-extrabold font-['Raleway-Black']">
          <div class="pb-3">Healthy & Fresh</div>
          <div>Food For You</div>
        </div>
        <div class="py-6">
          Create for lovers of healthy, delicious, and <br />
          non-obvious food.
        </div>
        <button class="bg-orange-400 hover:bg-orange-300 rounded-lg py-3 px-4">
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
        <img
          class="absolute inset-52 -left-96"
          src="../assets/images/hero-section-slide-food-1.png"
          alt=""
        />
      </div>
    </div>
    <img
      class="absolute -bottom-24"
      src="../assets/images/hero-section-food.png"
      alt=""
    />
  </div>
</template>

<style scoped></style>
