<template>
            <Header></Header>
            <Person_detail></Person_detail>
            <Content></Content>
            <el-backtop :bottom="100">
              <div
                style="
                  height: 100%;
                  width: 100%;
                  background-color: #f2f5f6;
                  box-shadow: 0 0 6px rgba(0, 0, 0, 0.12);
                  text-align: center;
                  line-height: 40px;
                  color: #1989fa;
                "
              >
                UP
              </div>
          </el-backtop>
        
      
</template>

<script>

import Header from '@/views/Header.vue'
import Person_detail from '@/views/Person_detail.vue'
import Content from '@/views/Content.vue'



export default {
  name: 'Index',
  data() {
    return {
      url_img: '../assets/2.jpg'
    }
  },
  components: {
      Header,
      Person_detail,
      Content
  }
}
</script>

<style type = "text/css" scope>

</style>
