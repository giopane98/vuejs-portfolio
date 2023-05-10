<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import EnjoyButton from './components/Enjoy-button.vue';
import Gallery from './components/Gallery.vue';
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="Ciao a tutti!" />
    </div>
  </header>

  <main>
    <Gallery 
    title="Prima"
    abstract="Questa sarà la mia prima foto"
    imageUrl="/images/neom-4q87Z96NBYg-unsplash.jpg"
    />
    <Gallery 
    title="Seconda" 
    abstract="Questa sarà la mia seconda foto"
    imageUrl="/images/neom-dMSYsXdwl9M-unsplash.jpg"
    />
    <Gallery 
    title="Terza" 
    abstract="Questa sarà la mia terza foto"
    imageUrl="/images/neom-epQdtCvBrc4-unsplash.jpg"
    />
    <EnjoyButton />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}


@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
