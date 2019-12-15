<template>
  <a class="page-nav" :href="address">
    <img class="nav-logo" :src="logo" background-size="cover" />
    <p>{{text}}</p>
  </a>
</template>

<script>
export default {
  props: ['address', 'text', 'logo']
}
</script>

<style>
.page-nav {
  padding: 5px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.nav-logo {
  width: 50px;
  height: 50px;
}
</style>
