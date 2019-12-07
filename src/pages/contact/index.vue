<template>
  <div class="page">
    <LogoHeader />
    <p>联系方式</p>
    <p>真真老师： 15238741696</p>
    <p>Summer老师：18790016676</p>

    <div class="weixins">
      <img src="/static/images/weixin1.png" mode="widthFix" />
      <img src="/static/images/weixin2.png" mode="widthFix" />
    </div>

    <map id="map" class="map" longitude="113.324520" latitude="23.099994" scale="14" :markers="markers"></map>
   </div>
</template>

<script>
  import PageContent from '@/components/PageContent'
  import LogoHeader from '@/components/LogoHeader'
  import ImageList from '@/components/ImageList'

  export default {
    data: {
      markers: [{
        id: 0,
        latitude: 23.099994,
        longitude: 113.324520,
        width: 50,
        height: 50
      }]
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

.weixins {
  display: flex;
  justify-content: space-between;
}

.weixins img {
  width: 49%;
}

.map {
  margin-top: 20px;
  width: 100%;
}
</style>
