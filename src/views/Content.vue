<template>
    <div id="content-outer">

        <el-row>
            <el-col :span="4"></el-col>
            <el-col :span="16">
                <el-timeline>
                    <el-timeline-item
                        v-for="(activity, index) in activities"
                        :key="index"
                        :timestamp="activity.timestamp"
                    >
                        {{ activity.content }}
                                <el-card shadow="hover" @click="testMethod(activity.timestamp)">
                                    <h4>Update Github template</h4>
                                    <p>Tom committed 2018/4/12 20:46</p>
                                  
                                </el-card>

                                <el-tag size="mini" type="info">Tag 3</el-tag>
                                <el-tag size="mini" type="warning">Tag 4</el-tag>
                    </el-timeline-item>
                </el-timeline>
            </el-col>
            <el-col :span="3"></el-col>
        </el-row>
        

    </div>
</template>

<script>

export default {
  name: 'Content',
  data() {
      return {
            activities: [
                {
                content: 'Event start',
                timestamp: '2018-04-15',
                },
                {
                content: 'Approved',
                timestamp: '2018-04-13',
                },
                {
                content: 'Success',
                timestamp: '2018-04-11',
                },  {
                content: 'Success',
                timestamp: '2018-04-11',
                },  {
                content: 'Success',
                timestamp: '2018-04-11',
                },  {
                content: 'Success',
                timestamp: '2018-04-11',
                },  {
                content: 'Success',
                timestamp: '2018-04-11',
                },  {
                content: 'Success',
                timestamp: '2018-04-11',
                },  {
                content: 'Success',
                timestamp: '2018-04-11',
                },  {
                content: 'Success',
                timestamp: '2018-04-11',
                },  {
                content: 'Success',
                timestamp: '2018-04-11',
                },
            ],
      }
  },
  methods: {
      testMethod(mes) {
          console.log(mes)
      }
  },
  components: {  }
}
</script>

<style scoped>

</style>
