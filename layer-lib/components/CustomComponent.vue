<template>
  <div style="background-color: aqua;" @click="onClick">CustomComponent</div>
</template>

<script setup>
const route = useRoute()

const onClick = () => {
  console.log('click on custom component in:',route.path)
}
</script>
