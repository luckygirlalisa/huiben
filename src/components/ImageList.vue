<template>
  <div class="images">
    <div class="image" v-for="image in images" v-bind:key="image">
        <img :src="image" mode="widthFix" />
    </div>
  </div>
</template>

<script>
export default {
  props: ['images']
}
</script>

<style>
.images {
  display: flex;
  flex-direction: column;
}

.image {
  width: 100%;
}

.image img {
  width: 100%;
}
</style>