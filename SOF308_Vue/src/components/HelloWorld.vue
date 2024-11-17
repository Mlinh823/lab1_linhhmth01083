<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="container">
  <button class="btn btn-danger">Danger</button>
  <button class="btn btn-warning">Warning</button>
  <button class="btn btn-success">Success</button>
  <button class="btn btn-info">Info</button>
  <button class="btn btn-primary">Primary</button>
  </div>
  </template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
