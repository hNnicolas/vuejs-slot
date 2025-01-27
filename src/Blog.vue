<template>
  <div class="container">
    <slot :date="date"></slot>
  </div>
</template>

<script setup lang="ts">

const date = Date()

</script>


<style scoped lang="scss">
.container {
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 20px;
  width: 500px;
  :slotted(h1) {
    color: gray;
  }
}
</style>
