<template>
  <div class="menu-wrapper">
    <el-menu router :default-active="onRoutes"
             background-color="#545c64"
             text-color="#fff"
             active-text-color="#ffd04b">
      <el-submenu index="1">
        <template slot="title">
          <span>前言</span>
        </template>
        <el-menu-item index="/SingleModel/Introduce">项目意义</el-menu-item>
        <el-menu-item index="/SingleModel/Plan">项目进度</el-menu-item>
        <el-menu-item index="/SingleModel/Demo">机器学习开胃菜</el-menu-item>
      </el-submenu>
      <el-menu-item index="/SingleModel/DataIntroduce">
        数据介绍
      </el-menu-item>
      <el-menu-item index="/SingleModel/training">30分钟后功率预测</el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  name: 'BarMenu',
  methods: {
  },
  computed: {
    onRoutes () {
      return this.$route.path
    }
  }
}
</script>

<style scoped>
.menu-wrapper {
  width: 100%;
}
</style>
