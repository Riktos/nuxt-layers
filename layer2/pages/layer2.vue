<template>
  <section class="layer2-page">
    <h1>Layer2 Технологии</h1>
    <div v-for="(item, index) in cards" :key="'item-' + index">
      <CardComponent
        :id="item.id"
        :title="item.title"
        :description="item.description"
      />
    </div>
  </section>
</template>

<script setup lang="ts">
import { reactive } from "vue";

const cardTemplate = {
  title: "КартаНазвание",
  description: "Описание для КартаОписание.",
};

const cards = reactive([]);
for (let i = 0; i < 10; i++) {
  cards.push({
    ...cardTemplate,
    id: i + 1,
  });
}
</script>

<style scoped>
</style>