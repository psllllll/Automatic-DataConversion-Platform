<template>
  <div class="app-container home">
    <el-row :gutter="20">
      <el-col :sm="24" :lg="24">
        <blockquote  style="font-size: 24px">
          <img src="@/assets/logo/logo.png" style="width:50px;height:50px" alt="">
          <div>欢迎来到数据转换平台！</div>
          <br />
        </blockquote>
        <hr />
      </el-col>
    </el-row>
    <el-row :gutter="20">
      <el-col :sm="24" :lg="12" style="padding-left: 20px">
       
        <p>
          <!--
          <el-button
            type="primary"
            icon="Cloudy"
            plain
            @click="goTarget('https://gitee.com/y_project/RuoYi-Vue')"
            >访问码云</el-button
          >

          -->
          <el-button
            icon="HomeFilled"
            plain
            >主页内容</el-button
          >
        </p>
      </el-col>

 
      
    </el-row>

   

  </div>
</template>

<script setup name="Index">
import useUserStore from '@/store/modules/user';
const user = useUserStore()
const version = ref('3.8.2')

function goTarget(url) {
  window.open(url, '__blank')
}
</script>

<style scoped lang="scss">


.app-container{
  background: linear-gradient(90.21deg, #eeeeee -5.91%, #c5ebc0 111.58%);
  opacity: 1;
}

.home {
  blockquote {
    padding: 10px 20px;
    margin: 0 0 20px;
    font-size: 17.5px;
    border-left: 5px solid #eee;
  }
  hr {
    margin-top: 20px;
    margin-bottom: 20px;
    border: 0;
    border-top: 1px solid #eee;
  }
  .col-item {
    margin-bottom: 20px;
  }

  ul {
    padding: 0;
    margin: 0;
  }

  font-family: "open sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  color: #676a6c;
  overflow-x: hidden;

  ul {
    list-style-type: none;
  }

  h4 {
    margin-top: 0px;
  }

  h2 {
    margin-top: 10px;
    font-size: 26px;
    font-weight: 100;
  }

  p {
    margin-top: 10px;

    b {
      font-weight: 700;
    }
  }

  .update-log {
    ol {
      display: block;
      list-style-type: decimal;
      margin-block-start: 1em;
      margin-block-end: 1em;
      margin-inline-start: 0;
      margin-inline-end: 0;
      padding-inline-start: 40px;
    }
  }
}
</style>

