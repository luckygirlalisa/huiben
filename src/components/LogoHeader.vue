<template>
  <div class="header">
    <div class="line left"></div>
    <div :class="logoClass">
      <img src="/static/images/logo.png" background-size="cover" />
      <p class="title" v-if="title">{{title}}</p>
    </div>
    <div class="line right"></div>
  </div>
</template>

<script>
export default {
  props: ['size', 'title'],
  computed: {
    logoClass: function () {
      return this.size === 'big' ? 'logo big' : 'logo'
    }
  }
}
</script>

<style>
.header {
  display: flex;
  align-items: center;
  margin-bottom: 20px;
}

.line {
  height: 3px;
  background-color: rgb(161, 183, 221);
  flex: 1;
}

.line.left {
  margin-right: 20px;
}

.line.right {
  margin-left: 20px;
}

.logo {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.logo img{
  height: 60px;
  width: 60px;
}

.logo.big img {
  height: 120px;
  width: 120px;
}

.title {
  margin-top: 10px;
}
</style>