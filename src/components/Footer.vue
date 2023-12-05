<script setup lang="ts"></script>

<template>
  <div class="bg-neutral-200">
    <div
      class="flex basis-1/3 flex-col bg-neutral-200 pb-12 pt-6 drop-shadow-md md:flex-row"
    >
      <!-- Footer Logo -->
      <div class="max-h-[72px] w-auto shrink-0 pl-4 md:pl-20">
        <img src="../assets/icons/logo.svg" />
      </div>
      <!-- Footer Navigation -->
      <div
        class="mb-6 ml-4 mt-3 flex basis-1/3 flex-col gap-4 md:items-center xl:flex-row xl:place-content-center xl:gap-14"
      >
        <a href="#about-us" class="font-semibold">ABOUT US</a>
        <a href="#menu" class="font-semibold">MENU</a>
        <a href="#contact" class="font-semibold">CONTACT</a>
      </div>
      <!-- Footer Engaging Text and Socials -->
      <div class="mx-4 mt-3 flex basis-1/3 flex-col">
        <div>
          <div>Stay up to date with our new openings, upcoming events</div>
          <div>seasonal specials and promotions. Check our socials.</div>
        </div>
        <div class="flex flex-row items-center gap-4 pt-6">
          <img
            class="hover:animate-pulse"
            src="../assets/icons/twitter-icon.svg"
            alt=""
          />
          <img
            class="hover:animate-pulse"
            src="../assets/icons/facebook-icon.svg"
            alt=""
          />
          <img
            class="hover:animate-pulse"
            src="../assets/icons/instagram-icon.svg"
            alt=""
          />
        </div>
      </div>
    </div>
    <div class="ml-4 py-6 md:ml-20 md:text-start">
      &copy; 2023 The Veggie King
    </div>
  </div>
</template>

<style scoped></style>
