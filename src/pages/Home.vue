<template>
  <div class="home">
      <div class="slide-left ">
        <UserInfo></UserInfo>
      </div>
      <Content class="slide-content"></Content>
  </div>
</template>
<script>
import UserInfo from '@/components/UserInfo.vue'
import Content from './content/Content.vue'
export default {
  components: {
    UserInfo,
    Content
  }
}
</script>
<style lang="scss" scoped>
@import '@/scss/base.scss';
.home{
  font-size: 16px;
  flex-wrap: wrap;
  background-color: #eaeaea;
  .slide-left {
    background-image: url('../assets/1d5cd579cce238bc27fc485f8cba71cd.jpg');
    background-repeat: no-repeat;
    background-position: 50%;
    background-size: cover;
    height: 100vh;
    width: 40%;
    position: fixed;
  }
  .slide-content {
    margin-left: 40%;
    width: 60%;
  }
  @media screen and (min-width: 100px) and (max-width: 1024px){
      .home {
        display: flex;
      }
      .slide-left {
        position: relative;
        width: 100%;
        height: 400px;
      }
      .slide-content {
        margin-left: 0;
        width: 100%;
      }
  }
}

</style>
