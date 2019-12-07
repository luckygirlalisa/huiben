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
        '/static/images/logo.png',
        '/static/images/logo.png',
        '/static/images/logo.png',
        '/static/images/logo.png'
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
