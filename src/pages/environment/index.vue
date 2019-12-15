<template>
  <div class="page">
    <LogoHeader />
    <p class="mb">小熊家绘本馆环境优美，藏书丰富。</p>
    <ImageList :images="images"/>
   </div>
</template>

<script>
  import PageContent from '@/components/PageContent'
  import LogoHeader from '@/components/LogoHeader'
  import ImageList from '@/components/ImageList'

  export default {
    data: {
      images: [
        '/static/images/environment-1.jpg',
        '/static/images/environment-2.jpg',
        '/static/images/environment-3.jpg',
        '/static/images/environment-4.jpg',
        '/static/images/environment-5.jpg',
        '/static/images/environment-6.jpg',
        '/static/images/environment-7.jpg'
      ]
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
</style>
