<template>
  <el-row class="navheader">
    <el-col :span="8" class="logo" v-show="logoIsShow">
      <el-col :span="2"><img src="../assets/hui.png" alt=""></el-col>
      <el-col :span="22"><p>区域定位管控系统</p></el-col>
    </el-col>
    <el-col :span="8" class="logo logo-hui" v-show="!logoIsShow">
      <el-col :span="2"><img src="../assets/hu.png" alt=""></el-col>
      <el-col :span="22"><p>区域定位管控系统</p></el-col>
    </el-col>
    <el-col :span="8" class="logo"></el-col>
    <el-col :span="8" class="navoption">
      <el-col :span="21">
        <p>
          <span>当前位置：<a href="">{{ position }}</a></span><span>{{localTime}}</span>
        </p>
        <p>
          <span class="nav-plan">正在计划点名中</span><span class="nav-plan-time">计划清点：{{}}</span>
        </p>
      </el-col>
      <el-col :span="3">
        <a href="" class="nav-mobile"><img src="../assets/mobile.png" alt=""></a>
      </el-col>
    </el-col>
  </el-row>
</template>

<script>
  var nowdate
  setInterval(function () {
    var nowdates = new Date()
    nowdate = nowdates.getFullYear()
    console.log(nowdate)
  }, 600)
  export default {
    name: 'navheader',
    data () {
      return {
        logoIsShow: true,
        position: '厂房第一监区',
        localTime: nowdate
      }
    }
  }
</script>

<style lang="scss">
.navheader{
  p{
    margin: 0;
  }
  height: 122px;
  color: #fff;
  font-size: 20px;
  .logo{
    padding: 30px;
    p{
      margin: 0;
      text-align: left;
      line-height: 54px;
      margin-left: 40px;
      font-size: 36px;
    }
  }
  .logo-hui{
    p{
      color: #bbb;
    }
  }
  .navoption{
    p{
      text-align: left;
    }
  }
}
</style>
