<template>
  <div class="page">
    <LogoHeader />
    <ImageList :images="images"/>
    <input class="input first" type="text" v-model="name" placeholder="姓名">
    <input class="input" type="text" v-model="phone" placeholder="电话">
    <input class="input" type="text" v-model="school" placeholder="学校">
    <input class="input" type="text" v-model="home" placeholder="住址">
    <button class="button" type="primary">提交</button>
   </div>
</template>

<script>
  import PageContent from '@/components/PageContent'
  import LogoHeader from '@/components/LogoHeader'
  import ImageList from '@/components/ImageList'

  export default {
    data: {
      images: [
        '/static/images/logo.png'
      ],
      name: '',
      school: '',
      phone: '',
      home: ''
    },
    components: {
      ImageList,
      PageContent,
      LogoHeader
    }
  }
</script>

<style>
.page {
  padding: 20px;
}

.mb {
  margin-bottom: 20px;
}

.input.first {
  border-top: 1rpx solid #D9D9D9;
}
.input {
  border-bottom: 1rpx solid #D9D9D9;
  border-left: none;
  border-right: none;
  padding: 10px 20px;
}
.button {
  margin-top: 10px;
}
</style>
