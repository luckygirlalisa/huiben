<template>
  <div @click="clickHandle">

    <div>
      <img class="banner" src="/static/images/main-picture.png" background-size="cover"/>
    </div>
    <LogoHeader title="小熊家绘本馆"></LogoHeader>

    <div class="main-nav">
      <menusection address="/pages/about/main" text="关于我们" logo="/static/images/logo/about-us.png"></menusection>
      <menusection address="/pages/environment/main" text="管内风采" logo="/static/images/logo/environment.png"></menusection>
      <menusection address="/pages/moment/main" text="精彩瞬间" logo="/static/images/logo/moment.png"></menusection>
    </div>
    <div class="main-nav">
      <menusection address="/pages/join-us/main" text="加入我们" logo="/static/images/logo/join-us.png"></menusection>
      <menusection address="/pages/club2/main" text="会员空间" logo="/static/images/logo/club.png"></menusection>
      <menusection address="/pages/contact/main" text="联系我们" logo="/static/images/logo/contact-us.png"></menusection>
    </div>

  </div>
</template>

<script>
import card from '@/components/card'
import menusection from '@/components/MenuSection'
import LogoHeader from '@/components/LogoHeader'

export default {
  data () {
    return {
      motto: 'Hello miniprograme',
      userInfo: {
        nickName: '小熊家绘本馆',
        avatarUrl: '/static/images/cartoon-bear.jpg'
      }
    }
  },

  components: {
    card,
    menusection,
    LogoHeader
  },

  methods: {
    bindViewTap () {
      const url = '../logs/main'
      if (mpvuePlatform === 'wx') {
        mpvue.switchTab({ url })
      } else {
        mpvue.navigateTo({ url })
      }
    },
    clickHandle (ev) {
      console.log('clickHandle:', ev)
      // throw {message: 'custom test'}
    }
  },

  created () {
    // let app = getApp()
  }
}
</script>

<style scoped>
.main-nav {
  margin: 20px 10% auto 10%;
  display: flex;
  justify-content: space-between;
  flex-wrap: nowrap;
}

.usermotto {
  margin-top: 150px;
}

.form-control {
  display: block;
  padding: 0 12px;
  margin-bottom: 5px;
  border: 1px solid #ccc;
}
.all{
  width:7.5rem;
  height:1rem;
  background-color:blue;
}
.all:after{
  display:block;
  content:'';
  clear:both;
}
.left{
  float:left;
  width:3rem;
  height:1rem;
  background-color:red;
}

.right{
  float:left;
  width:4.5rem;
  height:1rem;
  background-color:green;
}

.banner {
  height: 200px;
  width: 100%;
}
</style>
