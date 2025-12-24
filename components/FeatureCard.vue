<template>
  <div class="card">
    <img :src="img" alt="Feature" />
    <h3>{{ title }}</h3>
    <p>{{ description }}</p>
  </div>
</template>

<script>
export default {
  props: {
    img: { type: String, default: '/images/feature1.png' },
    title: { type: String, default: 'Feature Title' },
    description: { type: String, default: 'Feature description goes here.' }
  }
}
</script>

<style scoped>
.card {
  background: #fff;
  padding: 20px;
  border-radius: 10px;
  text-align: center;
  width: 300px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
}
.card img {
  width: 80px;
  margin-bottom: 15px;
}
.card h3 {
  margin-bottom: 10px;
}
</style>