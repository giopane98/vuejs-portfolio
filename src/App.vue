<script>
import Gallery from './components/Gallery.vue';

import worksData from './assets/works.json';

export default {
  data() {
    return {
      works: worksData,
    };
  },
   components: {
    Gallery,
  }
};

</script>

<template>
  <main>
  </main>


    <div id="works">
        <div v-for="work in works" :key="work.id">
          <Gallery
          :title="work.title"
          :abstract="work.description"
          :imageUrl="work.image_thumbnail"
          />
        </div>
      </div>

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
