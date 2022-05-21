<template>
  <header>
    <section>
      <div>
        <h1>Hello World!</h1>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic assumenda exercitationem explicabo nesciunt incidunt molestias saepe sint ex totam, laudantium earum rerum nostrum tempora porro quidem doloremque eos ipsam voluptate.
        </p>
      </div>
    </section>
    <picture>
      <img src="https://doodleipsum.com/500x500/abstract" />
    </picture>
  </header>
</template>

<style scoped>
header {
  display: grid;
  width: 100vw;
}

picture, section {
  display: grid;
  place-items: center;
}

picture {
  background-color: #339af0;
  padding: var(--size-8);
}

section div {
  padding: var(--size-8);
}

/* --md-n-above */
@media (min-width: 768px) {
  header {
    grid-template-columns: 1fr 1fr;
  }
}
</style>

