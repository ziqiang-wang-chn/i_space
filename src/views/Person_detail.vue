<template>
    <div id="detail-outer">
        <div class="detail-inner">
            <el-row>
                <el-col :offset="8" :span="3">
                    <el-avatar shape="circle" :size="135" fit="fill" :src="url"></el-avatar>
                </el-col>

                <el-col :span="5">
                <br>
                <br>
                    <p id="cinfo">看看我的生活</p>
                <br>
                    <p id="einfo">Look at my life</p>
                </el-col>
            </el-row>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Person_detail',
  data() {
      return {
          url: require('../assets/avatar.gif')
      }
  },
  components: {
  }
}
</script>

<style scoped>
    .detail-outer {
        width: 100%;
        height: 200px;
    }
    .detail-inner{
        width: 100%;
        padding-top: 190px;
        padding-bottom: 100px;
    }
    p{
        font-weight: bold;
        font-size: 30px;
    }
</style>