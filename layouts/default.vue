<template>
  <div>
    <div>
      <el-low :gutter="10">
        <el-col :sm="6"
          ><div class="grid-content bg-purple-light"><left-sidebar /></div
        ></el-col>
        <el-col :sm="12"
          ><div class="grid-content bg-purple"><nuxt /></div
        ></el-col>
        <el-col :sm="6"
          ><div class="grid-content bg-purple-light"><right-sidebar /></div
        ></el-col>
      </el-low>
      <el-col :sm="24">
        <div><Footer /></div>
      </el-col>
    </div>
  </div>
</template>

<script>
import LeftSidebar from '../components/LeftSidebar.vue'
import RightSidebar from '../components/RightSidebar.vue'
import Footer from '../components/Footer.vue'
export default {
  components: {
    LeftSidebar,
    RightSidebar,
    Footer,
  },
}
</script>
