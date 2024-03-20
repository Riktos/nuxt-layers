<template>
  <div class="card">
    <div class="card-body">
      <h5 class="card-title">{{ title }}</h5>

      <span class="card-number">{{ id }}</span>
      <p class="card-text">{{ description }}</p>
    </div>
  </div>
</template>

<script setup lang="ts">
interface Props {
  id: number
  title: string,
  description: string,
}

defineProps<Props>();

</script>

<style scoped>
.card {
  border: 1px solid #ddd;
  border-radius: 8px;
  overflow: hidden;
}

.card-img {
 width:100%;
 height:auto; 
 object-fit: cover;  
}

.card-body {
 padding:20px;   
}
  
.card-title {
 margin-bottom:12px; 
 font-size:20px;
}

.card-text{
 color:#666;
}
</style> 

