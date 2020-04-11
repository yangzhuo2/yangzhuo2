<template>
  <div class="user-info">
      <!-- <Icon type="md-search" /> -->
      <div class="user-box">
        <Avatar icon="ios-person" :size="85"  src="
        https://badegg.oss-cn-shanghai.aliyuncs.com/img/WechatIMG1.jpeg
        ">
        </Avatar>
        <div class="name">
          YangZhuo
        </div>
      </div>
      <h1 class="my-title">
          格物致知 知行合一
      </h1>
  </div>
</template>
<script>
import { Avatar } from 'view-design';
export default {
  components: {
    Avatar
  }
}
</script>
<style lang="scss" scoped>
@import '@/scss/base.scss';
.user-info {
  font-size: 12px;
  color: #fff;
    // flex-direction: column ;
    z-index: 2;
    margin: 0  auto;
    width: 85%;
    padding-top:20%;
    text-align: left;
    // height: 200px;
    .user-box {
      display: inline-block;
    // margin-top: 40px;
      text-align: center;
      .name {
        font-weight: 700;
        margin-top:12px;
        font-size: 16px;
        // margin-left: 15px;
      }

    }
    .my-title {
        font-weight: 700;
    }
    // justify-content: center;
}
</style>
