-/<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <navheader></navheader>
    <router-view></router-view>
    <menufooter></menufooter>
    <!--用户登录 star-->
    <div class="alertTip alertYHDL" v-show="false">
          <div class="alertBody " style="margin: -204px -316px;width: 632px;height: 408px;">
            <div class="bodyHead"><div class="title">用户登录</div><div class="close">X</div></div>
            <div class="bodyCon">
              <el-row class="menu_title_wrap">
                <el-col :span="6" >
                  <div style="height: 57px"></div>
                    <p>登录名：</p>
                  <div style="height:12px"></div>
                    <p>密码：</p>
                </el-col>
                <el-col :span="12">
                 <span class="tipHead">请民警登录或刷卡确认</span>
                  <input type="text">
                  <input type="text">
                </el-col>
                <el-col :span="6" style="height: 10px"></el-col>
              </el-row>
            </div>
            <div class="partsFoot">
              <div style="margin: 20px 2px;float: right">
                <div class="sure">确定</div>
              </div>
            </div>
          </div>
    </div>
    <!--用户登录 end-->

    <!--监区选择 star-->
    <div class="alertTip alertJQXZ" v-show="false">
      <div class="alertBody " style="margin: -204px -316px;width: 632px;height: 270px;">
        <div class="bodyHead"><div class="title">监区选择</div><div class="close">X</div></div>
        <div class="bodyCon">
          <el-row>
            <el-col :span="5" >
              <div style="width:10px;"></div>

              <div class="areas">一监区</div>
            </el-col>
            <el-col :span="5" >
              <div style="width:10px;"></div>

              <div class="areas">二监区</div>
            </el-col>

            <el-col :span="5" >
              <div style="width:10px;"></div>

              <div class="areas">三监区</div>
            </el-col>
            <el-col :span="5" >
              <div style="width:10px;"></div>

              <div class="areas">四监区</div>
            </el-col>
          </el-row>
        </div>
        <div class="partsFoot">
          <div style="margin: 20px 2px;float: right">
            <div class="sure">确定</div>
          </div>
        </div>
      </div>
    </div>
    <!--监区选择 end-->

    <!--报警信息 star-->
    <div class="alertTip alertBJXX" v-show="false">
      <div class="alertBody " style="margin: -222px -400px;width: 800px;height: 444px;">
        <div class="bodyHead"><div class="title">报警信息</div><div class="close">X</div></div>
        <div class="bodyCon" style="height: 312px;">
          <div class="lists" v-show="true">
            <el-row>

                <div class="tipName">报警事件名称</div>
                <el-row>
                  <el-col :span="4"  >

                    <div ><img width="100%"  src="./assets/crimal_1_03.jpg" alt=""></div>
                    <span>张学友 <br> 123456</span>
                  </el-col>
                  <el-col :span="4"  >
                    <div ><img width="100%"  src="./assets/crimal_1_03.jpg" alt=""></div>
                    <span>张学友 <br> 123456</span>
                  </el-col>
                  <el-col :span="4"  >
                    <div ><img width="100%"  src="./assets/crimal_1_03.jpg" alt=""></div>
                    <span style="color: red">张学友 <br> 123456</span>
                  </el-col>
                  <el-col :span="4"  >
                    <div ><img width="100%"  src="./assets/crimal_1_03.jpg" alt=""></div>
                    <span>张学友 <br> 123456</span>
                  </el-col>
                  <el-col :span="4"  >
                    <div ><img width="100%"  src="./assets/crimal_1_03.jpg" alt=""></div>
                    <span>张学友 <br> 123456</span>
                  </el-col>
                </el-row>

            </el-row>
            <el-row >
              <el-col :span="8" style="height: 10px"></el-col>
              <el-col :span="8" >
                <div class="pages">
                  <span class="pageControl"><img src="./assets/q1.png" alt=""/></span>
                  <span class="pagesText">11/30</span>
                  <span class="pageControl"><img src="./assets/q2.png" alt=""/></span>
                </div>
              </el-col>
              <el-col :span="8" style="height: 10px"></el-col>
            </el-row>
          </div>
          <div class="details" v-show="false" >
            <el-row>
              <el-col :span="6" style="height:1px;">
              </el-col>
              <el-col :span="12" >
                <div class="tipName">报警事件名称</div>
                <div style="height:18px;"></div>
                <el-row>
                  <el-col :span="10" >
                    <div>
                      <img src="/static/img/crimal_1_03.5a235b3.jpg" alt="">
                    </div>
                  </el-col>
                  <el-col :span="14" >
                    <p>姓名：李栓怪</p>
                    <p>罪犯编号：123456</p>
                    <p>报警区域：厕所</p>
                    <p>报警时间：2017-12-11</p>
                  </el-col>
                </el-row>
              </el-col>
              <el-col :span="6" style="height:1px;" >
              </el-col>
            </el-row>
            <el-row >
              <el-col :span="8" style="height: 10px"></el-col>
              <el-col :span="8" >
                <div class="pages">
                  <span class="pageControl"><img src="./assets/q1.png" alt=""/></span>
                  <span class="pagesText">11/30</span>
                  <span class="pageControl"><img src="./assets/q2.png" alt=""/></span>
                </div>
              </el-col>
              <el-col :span="8" style="height: 10px"></el-col>
            </el-row>
          </div>
         </div>
        <div class="partsFoot">
          <div style="margin: 20px 2px;float: right">
            <div class="sure">处理</div>
          </div>
        </div>
      </div>
    </div>
    <!--报警信息 end-->

    <!--实时流动 star-->
    <div class="alertTip alertSSLD" v-show="false">
      <div class="alertBody " style=" margin: -290px -440px;width: 880px;height: 580px;">
        <div class="bodyHead"><div class="title">实时流动</div><div class="close">X</div></div>
        <div class="bodyCon" style="height: 466px;">
          <el-row>
            <el-col :span="12" >
              <el-col :span="7" >
                  <div class="moveCrimal">
                    <div><img src="./assets/crimal_1_03.jpg" width="70%" height="100" alt=""></div>
                    <span>张家辉 <br> 13:23出门</span>
                  </div>
              </el-col>
              <el-col :span="7" >
                <div class="moveCrimal">
                <div><img src="./assets/crimal_1_03.jpg" width="70%" height="100" alt=""></div>
                  <span>张家辉 <br> 13:23出门</span>
                </div>
              </el-col>
              <el-col :span="7" >
                <div class="moveCrimal">
                  <div><img src="./assets/crimal_1_03.jpg" width="70%" height="100" alt=""></div>
                  <span>张家辉 <br> 13:23出门</span>
                </div>
              </el-col>
              <el-col :span="7" >
                <div class="moveCrimal">
                  <div><img src="./assets/crimal_1_03.jpg" width="70%" height="100" alt=""></div>
                  <span>张家辉 <br> 13:23出门</span>
                </div>
              </el-col>
              <el-col :span="7" >
                <div class="moveCrimal">
                  <div><img src="./assets/crimal_1_03.jpg" width="70%" height="100" alt=""></div>
                  <span>张家辉 <br> 13:23出门</span>
                </div>
              </el-col>
              <el-col :span="7" >
                <div class="moveCrimal">
                  <div><img src="./assets/crimal_1_03.jpg" width="70%" height="100" alt=""></div>
                  <span>张家辉 <br> 13:23出门</span>
                </div>
              </el-col>
              <el-col :span="7" >
                <div class="moveCrimal">
                  <div><img src="./assets/crimal_1_03.jpg" width="70%" height="100" alt=""></div>
                  <span>张家辉 <br> 13:23出门</span>
                </div>
              </el-col>
              <el-col :span="7" >
                <div class="moveCrimal">
                  <div><img src="./assets/crimal_1_03.jpg" width="70%" height="100" alt=""></div>
                  <span>张家辉 <br> 13:23出门</span>
                </div>
              </el-col>
              <el-col :span="7" >
                <div class="moveCrimal">
                  <div><img src="./assets/crimal_1_03.jpg" width="70%" height="100" alt=""></div>
                  <span>张家辉 <br> 13:23出门</span>
                </div>
              </el-col>
            </el-col>
            <el-col :span="12">
              <el-col :span="7" style="height: 10px">

              </el-col>
              <el-col :span="10" >
                <div class="moveCrimal">
                  <div style="height:50px;"></div>
                  <div><img src="./assets/crimal_1_03.jpg" width="100%" height="250" alt=""></div>
                  <span style="font-size: 20px;font-weight: 800">张家辉 <br> 13:23出门 <br> 11人次</span>
                </div>
              </el-col>
              <el-col :span="7" style="height: 10px" >

              </el-col>
            </el-col>

          </el-row>
        </div>
        <div class="partsFoot" style="height: 70px">
          <div style="margin: 20px 2px;float: right">
            <div class="sure">确定</div>
          </div>
        </div>
      </div>
    </div>
    <!--实时流动 end-->

    <!--已点名单 star-->
    <div class="alertTip alertYDMD" v-show="false">
      <div class="alertBody " style="margin: -330px -550px;width: 1100px;height: 660px;">
        <div class="bodyHead"><div class="title">已点名单</div><div class="close">X</div></div>
        <div class="bodyCon" style="height: 514px;">
          <el-col :span="12" >
            <el-col :span="12" >
                <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>



          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
          <el-col :span="12" >
            <el-col :span="12" >
              <div class="tab">条目一</div>
            </el-col>
            <el-col :span="12" >
              <div class="tab">条目一内容</div>
            </el-col>
          </el-col>
        </div>
        <el-row >
          <el-col :span="8" style="height: 10px"></el-col>
          <el-col :span="8" >
            <div class="pages">
              <span class="pageControl"><img src="./assets/q1.png" alt=""/></span>
              <span class="pagesText">11/30</span>
              <span class="pageControl"><img src="./assets/q2.png" alt=""/></span>
            </div>
          </el-col>
          <el-col :span="8" style="height: 10px"></el-col>
        </el-row>
      </div>
    </div>
    <!--已点名单 end-->
  </div>
</template>

<script>
import navheader from './components/navheader.vue'                  // 引入组件头部导航
import menufooter from './components/menufooter.vue'                // 引入组件底部菜单
export default {
  name: 'app',
  components: {
    navheader: navheader,         // 引入组件头部导航
    menufooter: menufooter        // 引入组件底部菜单
  }
}
</script>

<style>
body{
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100%;
  background: url('./assets/bg.png');
  background-repeat: no-repeat;
  background-size: 100% 100%;
}

.alertTip {
  position: absolute;
  width: 100%;
  height: 100%;
  z-index: 9999;
  top: 0;
  background: rgba(0, 0, 0, 0.78);
}
.alertTip .title {
  font-size: 25px;
  font-weight: 800;
  color: #1d68e8;
  text-shadow: 2px 2px 2px #fff;
  line-height: 45px;
  text-indent: 15px;
  float: left;
}
.alertTip .bodyHead {
  width: 100%;
  height: 46px;
  background: #c5cfdb;
}
.alertTip .bodyCon {
  height: 240px;
  padding: 20px;
}
.alertTip .partsFoot {
  width: 100%;
  height: 84px;
  /* margin-top: -48px; */
  background: #c5cfdb;
}
.alertTip .sure {
  width: 126px;
  height: 40px;
  background: #004bdc;
  text-align: center;
  color: white;
  font-size: 20px;
  line-height: 36px;
  letter-spacing: 2px;
  float: right;
  margin: 0px 35px;
}
.alertTip .alertBody{

    position: absolute;
    top: 50%;
    left: 50%;
  background: white;
  }
.alertTip  .close{
    float: right;
    font-weight: 900;
    font-size: 30px;
    margin: 0px 16px;
    color: #1d68e8;
  }



/*用户登录*/

.alertYHDL input{
  width:100%;
  margin:20px 0px;
  height:40px;
  border: 1px solid rgba(0, 0, 0, 0.38);
}
.alertYHDL .tipHead{
    display: inline-block;
    height: 60px;
    font-size: 20px;
    line-height: 70px;

  }
.alertYHDL p{
  font-size: 23px;
  text-align: right;
}
/*监区选择*/
.alertJQXZ .areas{
  width:100%;
  height: 50px;
  color: blue;
  border: 1px solid;
  font-size: 21px;
  text-align: center;
  line-height: 51px;
}
.alertJQXZ .el-col-5 {
  padding: 10px;
}
.alertJQXZ .bodyCon{
  height: 99px;
  padding: 20px
}

/*报警信息*/
 .alertBJXX p{
   text-align: left;
   font-size: 19px;
   color: red;
   font-weight: 800;
   height:15px;
  }
.alertBJXX .tipName{
  display: inline-block;
  height: 39px;
  font-size: 22px;
  color: rgba(0, 0, 255, 0.72);
  font-weight: 800;
   }
.alertBJXX .pages{
  width: 273px;
  height: 50px;
  margin: 18px auto;
}
.alertBJXX .pageControl{

}
.alertBJXX .pagesText {
  font-size: 24px;
  display: inline-block;
  width: 155px;
  text-align: center;
}
  .lists span{
    font-weight: 800;
    font-size: 20px;
  }
.alertBJXX .el-col-4 {
  width: 16.66667%;
  margin: 0px 12px;
}


  /*实时流动*/
  .alertSSLD .moveCrimal{
    margin:6px 0px;
  }
.alertSSLD span{
  color: black;
}
/*已点名单*/
.alertYDMD .pages{
  width: 273px;
  height: 50px;
  margin: 18px auto;
}
.alertYDMD .pageControl{

}
.alertYDMD .pagesText {
  font-size: 24px;
  display: inline-block;
  width: 155px;
  text-align: center;
}
.alertYDMD .tab{
  width: 100%;
  border: 1px solid rgb(0, 0, 0);
  height: 33px;
  font-size: 18px;
  font-weight: 800;
  line-height: 33px;
}
</style>
