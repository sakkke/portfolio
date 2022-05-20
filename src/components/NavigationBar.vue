<template>
  <nav>
    <ul>
      <li><router-link to="/">Home</router-link></li>
      <li><router-link to="/about">About</router-link></li>
      <li><router-link to="/apps">Apps</router-link></li>
      <li><router-link to="/links">Links</router-link></li>
    </ul>
  </nav>
</template>

<style scoped>
a {
  margin-block: 0;
  margin-inline: 0;
  padding-block: 0;
  padding-inline: 0;
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

