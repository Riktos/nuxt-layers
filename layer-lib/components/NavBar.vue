<template>
  <nav class="navbar">
    <div class="container">
      <a href="/" class="navbar-brand">Мой Сайт</a>
      <ul class="navbar-nav">
        <li><NuxtLink to="/">Главная</NuxtLink></li>
        <li v-for="route in routes" :key="route.toString()">
          <NuxtLink :to="route">{{route}}</NuxtLink>
        </li>
      </ul>
    </div> 
  </nav>
</template>

<script setup lang="ts">
interface Props {
  routes: string[]
}

 defineProps<Props>()

// Здесь могут быть скрипты или импорты
</script>

<style scoped>
.navbar {
  background-color:#343a40;
  color:white;
  padding:16px;
}

.container {
  display:flex;
  justify-content: space-between;
  align-items:center;    
}

.navbar-brand{
 font-size:24px;   
 text-decoration:none;
 color:white;
}

.navbar-nav{
 list-style-type:none;
 padding-left:0; 
}

.navbar-nav li{
 display:inline-block;  
 margin-right:20px;
}
 
 .navbar-nav li a{
   text-decoration:none;
   color:white;/* Белые ссылки */
 }
 
 .navbar-nav li a:hover{
   text-decoration:none;
   color:#ccc;/* Цвет ссылок при наведении */
 }
</style> 
