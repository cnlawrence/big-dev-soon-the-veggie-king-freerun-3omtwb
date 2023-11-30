<script setup lang="ts"></script>

<template>
  <div class="bg-neutral-200">
    <div class="flex flex-row bg-neutral-200 pb-10 pt-6 drop-shadow-md">
      <!-- Footer Logo -->
      <div class="mb-8 ml-20 flex h-12 flex-auto flex-row">
        <img src="../assets/icons/logo.svg" />
      </div>
      <!-- Footer Navigation -->
      <div class="my-3 flex flex-auto flex-row place-content-center gap-14">
        <a href="#about-us" class="font-semibold">ABOUT US</a>
        <a href="#menu" class="font-semibold">MENU</a>
        <a href="#contact" class="font-semibold">CONTACT</a>
      </div>
      <!-- Footer Engaging Text and Socials -->
      <div class="mt-3 flex flex-auto flex-col">
        <div>
          <div>Stay up to date with our new openings, upcoming events</div>
          <div>seasonal specials and promotions. Check our socials.</div>
        </div>
        <div class="flex flex-row gap-4 pt-6">
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
    <div class="ml-20 py-6">&copy; 2023 The Veggie King</div>
  </div>
</template>

<style scoped></style>
