<script setup> 
/* defineProps = che il mio progetto vue avrà delle proprietà che cambieranno */
defineProps({
  title: String,
  abstract: String,
  imageUrl: String,
})
</script>

<template>
    <div class="section">
      <div class="image">
         <img :src="imageUrl" width="125" height="125" />
      </div>
      <div class="video-text">
        <h1>{{ title }}</h1>
        <p class="description">{{ abstract }}</p>
      </div>
    </div>
</template>

<style scoped>

img {
  display: block;
  border-radius: 100%;
}

.section {
  background-color: #F2F2FF;
  border-radius: 5px;
  margin-bottom: 1.5rem;
  padding: 1rem;
  display: flex;
  align-items: center;
}

h1 {
  font-size: 1.4rem;
  color: #9898FF;
  font-weight: 800;
}
.description {
  font-size: 1.2rem;
  font-weight: 300;
  color: #7878ff;
  margin-top: -5px;
}

.video-text{
  margin-left: 2rem;
}
</style>
