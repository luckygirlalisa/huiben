<template>
  <PageContent>
    <LogoHeader size="big" ></LogoHeader>
    <p class="text">济源市小熊家绘本馆，是一家由学前教育及相关专业人员组成的专业团队，致力于为适龄儿童提供最优质的的中英文早期阅读服务。管内环境幽雅，藏书丰富，为家长省去大量买书资金和精力，更有专业指导老师，帮助家长为孩子选择适合自己的书，开设有中英文阅读指导，丰富的周末故事会、户外活动、亲子游戏、专家讲座等。</p>
  </PageContent>
</template>

<script>
import PageContent from '@/components/PageContent'
import LogoHeader from '@/components/LogoHeader'

export default {
  components: {
    PageContent,
    LogoHeader
  }
}
</script>

<style>
.text {
  padding: 10px;
}
</style>
