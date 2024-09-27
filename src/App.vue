<template>
  <v-app>
    <v-app-bar flat>
      <v-app-bar-title>chance.dev</v-app-bar-title>
      <v-btn variant="text" @click="scrollToSection('#home', 300)">Home</v-btn>
      <v-btn variant="text" @click="scrollToSection('#about', 400)">About</v-btn>
      <v-btn variant="text" @click="scrollToSection('#projects', 100)">Projects</v-btn>
      <v-btn variant="text" @click="scrollToSection('#contact', 50)">Contact</v-btn>
    </v-app-bar>
    <v-main class="main">
      <router-view />
    </v-main>
  </v-app>
</template>

<script lang="ts" setup>
function scrollToSection(selector: string, offset: number = 100): void {
  const target = document.querySelector(selector);
  if (target) {
    const targetPosition = target.getBoundingClientRect().top + window.scrollY - offset; // Adjust by offset
    window.scrollTo({
      top: targetPosition,
      behavior: 'smooth' // Enable smooth scrolling
    });
  }
}
</script>

<style>
</style>
