<template>
  <a class="page-nav" :href="address">
    <img class="nav-logo" src="/static/images/user.png" background-size="cover" />
    <p class="about-us">{{text}}</p>
  </a>
</template>

<script>
export default {
  props: ['address', 'text']
}
</script>

<style>
.page-nav {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.nav-logo {
  width: 50px;
  height: 50px;
}
</style>
