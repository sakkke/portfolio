<script setup lang="ts">
import { GridIcon, HomeIcon, Link2Icon, UserIcon } from '@vue-icons/feather'
</script>

<template>
  <nav>
    <ul>
      <li><router-link :class="{ 'current-path': this.$route.path === '/' }" to="/">Home <HomeIcon /></router-link></li>
      <li><router-link :class="{ 'current-path': this.$route.path === '/about' }" to="/about">About <UserIcon /></router-link></li>
      <li><router-link :class="{ 'current-path': this.$route.path === '/apps' }" to="/apps">Apps <GridIcon /></router-link></li>
      <li><router-link :class="{ 'current-path': this.$route.path === '/links' }" to="/links">Links <Link2Icon /></router-link></li>
    </ul>
  </nav>
</template>

<style scoped>
/* router-link */
a {
  color: inherit;
  display: flex;
  gap: var(--size-1);
  margin-block: 0;
  margin-inline: 0;
  padding-block: 0;
  padding-inline: 0;
}

/* router-link:hover */
a:hover {
  text-decoration: none;
}

li, ul {
  padding-left: 0;
}

nav {
  background-color: var(--surface-2);
  box-shadow: var(--shadow-1);
  display: grid;
  padding: var(--size-4) 0;
  place-items: center;
  width: 100%;
}

ul {
  display: flex;
  flex-direction: column;
  gap: var(--size-4);
  list-style-type: none;
}

.router-link-active {
  color: var(--blue-5);
}

/* --md-n-above */
@media (min-width: 768px) {
  ul {
    flex-direction: row;
  }
}
</style>

