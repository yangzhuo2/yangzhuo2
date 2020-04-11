<template>
  <div class="content">
    <div class="content-item" v-for="(itemm,key) in Data" :key="'xxxx;' + key">
      <h2>python爬虫脚本</h2>
      <p>
        <Icon type="md-time" />
        <span>2019-04-20 : 12:00:00</span> |
        <Icon type="md-pricetag" />
        <span>
          <Tag color="primary" >Python</Tag>
          <Tag color="primary" >JavaSript</Tag>
        </span>
      </p>
      <div class="content-item-logo" >
        <img src="https://badegg.oss-cn-shanghai.aliyuncs.com/img/43vvmv.jpg"
        alt="">
      </div>
      <div class="content-item-desc">
        Lx is a simple & clear & elegant hexo theme.
        Languages: 中文,English
        Current version: V0.3.9
        Source code on GitHub: https://github.com/blleng/hexo-theme-lx
      </div>
      <div class="content-item-button">
        <Button type="info" class="item-button" size='small'>
          继续阅读
        </Button>
      </div>
    </div>
  </div>
</template>
<script>
import { Icon,Tag,Button } from 'view-design';
export default {
  components: {
    Icon,
    Tag,Button
  },
  data () {
    return {
      Data: [1,2]
    }
  }
}
</script>
<style lang="scss" scoped>
@import '@/scss/base.scss';
  .content {
    padding: 10px;
    .content-item {
      margin: 20px 0;
      background-color: #fff;
      border-radius: 20px;
      text-align: left;
      font-size: 12px;
      padding: 15px 30px;
      h2 {
        font-weight: 700;
      }
      p {
        margin: 10px 0;
        i {
          margin-right: 7px;
        }
      }
      .content-item-logo {
        margin-bottom: 30px;
        img {
          // border:1px solid #ccc;
            padding: 3px;
            border: 1px solid #dedede;
           width: 100%;
          //  height: 390px;
        }
      }
      .content-item-button {
        text-align: right;
        .item-button {
          font-size: 10px;
        }
      }
    }
  }
</style>
