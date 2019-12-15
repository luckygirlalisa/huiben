<template>
   <PageContent>
       <LogoHeader />
       <div class="content">
         <p class="text">敬请期待</p>
       </div>
   </PageContent>
</template>

<script>
  import PageContent from '@/components/PageContent'
  import LogoHeader from '@/components/LogoHeader'

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
      PageContent,
      LogoHeader
    }
  }
</script>

<style>
.content {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>

