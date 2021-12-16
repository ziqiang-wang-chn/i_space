<template>
<el-affix :offset="0">
    <el-header>
      <el-row>
        <el-col :span="1"> <div style="font-weight:bold;">I_Space</div> </el-col>
        <el-col :span="1" :offset="16"> <div><el-link :underline="false" href="/">首页</el-link></div> </el-col>
        <el-col :span="1"> <div><el-link :underline="false">相册</el-link></div> </el-col>
        <el-col :span="1"> <div><el-link :underline="false">网盘</el-link></div> </el-col>
        <el-col :span="1"> <div><el-link :underline="false">链接</el-link></div> </el-col>
        <el-col :span="1"> <div><el-link :underline="false">关于我</el-link></div> </el-col>
        <el-col :span="2"> <div><el-link :underline="false" href="https://github.com/ziqiang-wang-chn">GitHub</el-link></div> </el-col>
      </el-row>          
    </el-header>
</el-affix>
</template>


<script>

export default {
  name: 'Header',
  components: {
  }
}
</script>


<style scoped>
.el-header {
  background-color: transparent;
  line-height: 60px;
  height: 60px;
}
</style>