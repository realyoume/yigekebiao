<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <div style="display: flex;justify-content: center;align-items: center;">
      <div style="width:500px">
        
        <el-row :gutter="20" v-for="(course, index) in courseData" :key="index" style="margin-top:20px">
          <el-col :span="8"><span style="font-size:16px;font-family:Microsoft Yahei">{{course.time}}</span></el-col>
          <el-col :span="8"><span style="font-size:16px;font-family:Microsoft Yahei">{{course.name}}</span></el-col>
          <el-col :span="8"><span style="font-size:16px;font-family:Microsoft Yahei">{{course.address}}</span></el-col>
        </el-row>

        <el-row :gutter="20" style="margin-top:70%" >
          <el-col :span="6"><el-button icon="el-icon-arrow-left" circle></el-button></el-col>
          <el-col :span="6"><el-button icon="el-icon-s-comment" circle></el-button></el-col>
          <el-col :span="6"><el-button icon="el-icon-menu" circle></el-button></el-col>
          <el-col :span="6"><el-button icon="el-icon-arrow-right" circle></el-button></el-col>
        </el-row>

      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{
      msg: "今天是周一，开启元气满满的一周",
      courseData: [{
            time: '8:00 - 9:00',
            name: '软件质量管理',
            address: '教学楼101'
          }, {
            time: '10:00 - 11:45',
            name: '人机交互系统',
            address: '教学楼202'
          }, {
            time: '15:00 - 16:00',
            name: '羽毛球',
            address: '运动馆501'
          }]
    }
  }
}
</script>