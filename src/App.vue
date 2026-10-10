<!--
Name: Jacob Lunsford
Date: 10/09/2026
Assignment: Vue 3 + Vite Application
Description: 
-->

<template>
  <h1 class="main-header">Jacob’s Vite + Vue Assignment</h1>

  <p class="intro-text">
    This application was created using Vue 3 and Vite.
  </p>

  <h2 class="sub-header">About Me</h2>
  <p class="about-text">My name is Jacob Lunsford.</p>

  <button class="counter-btn" @click="count++">
    Clicked {{ count }} times
  </button>

  <ul class="info-list">
    <li>Vue 3</li>
    <li>Vite</li>
    <li>Netlify Deployment</li>
  </ul>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<style>
.main-header {
  color: #42b883;
  font-size: 3rem;
  font-weight: bold;
}

.sub-header {
  margin-top: 20px;
  font-size: 2rem;
}

.counter-btn {
  margin-top: 20px;
  padding: 10px 20px;
  background: black;
  color: white;
  border: none;
  cursor: pointer;
}

.counter-btn:hover {
  background: #333;
}

.info-list {
  margin-top: 20px;
  list-style-type: square;
}

.intro-text,
.about-text {
  font-size: 1.2rem;
}
</style>
