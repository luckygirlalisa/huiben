<template>
  <div class="page">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: ['text']
}
</script>

<style>
.page {
  padding: 20px;
}
</style>
