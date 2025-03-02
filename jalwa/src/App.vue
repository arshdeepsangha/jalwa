<script setup lang="ts">
import { RouterView } from 'vue-router'
</script>

<template>
  <div class="header"></div>
  <RouterView />
  <div class="footer"></div>
</template>

<style scoped>
.header {
  height: 50px;
  background-color: #333;
  color: white;
  text-align: center;
  line-height: 50px;
}
.footer {
  height: 50px;
  background-color: #333;
  color: white;
  text-align: center;
  line-height: 50px;
}
</style>
