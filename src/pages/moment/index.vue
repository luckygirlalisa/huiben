<template>
  <div class="page">
    <LogoHeader />
    <p class="mb">小熊家绘本馆会不定期举办丰富的活动，故事分享会、家长课堂、以及各种旅游等。</p>
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
        '/static/images/moment-1.jpg',
        '/static/images/moment-2.jpg',
        '/static/images/moment-3.jpg',
        '/static/images/moment-4.jpg',
        '/static/images/moment-5.jpg'
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
