<script setup lang="ts">
import NavigationBar from './components/NavigationBar.vue'
</script>

<template>
  <NavigationBar />
  <router-view />
</template>

<style>
@import 'open-props/style';
@import 'open-props/normalize';

#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  place-items: center;
}

/* router-view */
#app > *:nth-child(2) {
  flex-grow: 1;
}
</style>

