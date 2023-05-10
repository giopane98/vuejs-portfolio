<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
    <div class="btn-enjoy">
      <p class="button">Scopri di più</p>
    </div>
</template>

<style scoped>
.btn-enjoy {
  background-color: #9898FF;
  border-radius: 40px;
  padding: 1rem;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 220px;
  height: 50px;
}
.button {
  font-size: 1.2rem;
  color: white;
  font-weight: 400;
}
</style>
