<script setup lang="ts">
import { ref } from 'vue';
import Gift from './components/Gift.vue'
import TreeVue from './components/Tree.vue';
import Card from './components/Card.vue'
const treeVisibleClass = ref('tree--hidden')
const cardOffsetClass = ref('card--hidden')
const handleClickGift = () => {
  treeVisibleClass.value = 'tree--visible'
  cardOffsetClass.value = 'card--visible'
}
</script>

<template>
  <div class="page">
    <Gift @click="handleClickGift" class="test"></Gift>
    <TreeVue :class="treeVisibleClass"></TreeVue>
    <Card :class="cardOffsetClass"></Card>
  </div>
</template>

<style scoped>
.page {
  height: 100vh;
  width: 100%;
  overflow: hidden;
  background-color: var(--blue);
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}
.tree--visible {
  transition: 500ms opacity ease-in-out;
  transition-delay: 250m;
  opacity: 1;
  z-index: 0;
}
.tree--hidden {
  opacity: 0;
  z-index: -1;
}
.card--hidden {
  transform: translate(-50%, 100%);
}
.card--visible {
  transform: translate(-50%, 50%);
  transition: transform 500ms ease-in-out;
}
</style>
