<script setup lang="ts">
import Navigation from "./components/Navigation.vue";
</script>

<template>
  <Navigation />
  <div class="footer">
    <a href="https://bigdevsoon.me" target="_blank" rel="noopener noreferrer"
      >Project by cnlawrence</a
    >
    |
    <span
      >Built with ❤️ by
      <a
        href="https://github.com/cnlawrence/big-dev-soon-the-veggie-king-freerun-3omtwb"
        >[Me]</a
      >
    </span>
  </div>
</template>

<style scoped>
/* This is an example CSS file, feel free to remove/edit it anytime */
.footer {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 10px;
  text-align: center;
}

.footer a {
  font-size: 14px;
  font-weight: bold;
  text-decoration: none;
}

.footer span {
  font-size: 14px;
}
</style>
