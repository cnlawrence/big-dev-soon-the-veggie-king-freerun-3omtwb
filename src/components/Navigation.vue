<script setup lang="ts">
import { ref } from "vue";

const isOpen = ref(false);
</script>

<template>
  <div class="flex max-h-[72px] flex-row bg-neutral-50 drop-shadow-2xl">
    <!-- Logo -->
    <div class="my-4 ml-4 flex flex-auto shrink-0 flex-row md:ml-10 lg:ml-20">
      <img src="../assets/icons/logo.svg" />
    </div>
    <!-- Nav Links -->
    <div class="my-6 mr-32 hidden gap-10 md:flex">
      <a href="#about-us" class="duration-400 font-semibold hover:scale-105"
        >ABOUT US</a
      >
      <a href="#menu" class="duration-400 font-semibold hover:scale-105"
        >MENU</a
      >
      <a href="#contact" class="duration-400 font-semibold hover:scale-105"
        >CONTACT</a
      >
    </div>
    <!-- Mobile Nav Control -->
    <div class="flex pr-4 md:hidden" @click="isOpen = !isOpen">
      <img
        :class="{ hidden: isOpen }"
        src="../assets/icons/menu-icon.svg"
        alt=""
      />
      <img
        :class="{ hidden: !isOpen }"
        src="../assets/icons/close-menu-icon.svg"
        alt=""
      />
    </div>
  </div>
  <!-- Mobile Nav -->
  <div
    id="mobile-menu"
    class="absolute z-50 w-full bg-neutral-50 text-center drop-shadow-2xl md:hidden"
    :class="{ hidden: !isOpen }"
  >
    <ul class="bg-white p-8">
      <li class="py-6">
        <a href="#about-us" class="duration-400 font-semibold hover:scale-105"
          >ABOUT US</a
        >
      </li>
      <li class="py-6">
        <a href="#menu" class="duration-400 font-semibold hover:scale-105"
          >MENU</a
        >
      </li>
      <li class="py-6">
        <a href="#contact" class="duration-400 font-semibold hover:scale-105"
          >CONTACT</a
        >
      </li>
    </ul>
  </div>
</template>

<style scoped></style>
