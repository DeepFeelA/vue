<template>
  <div id="app">
   <!-- <el-container style="height: 600px; border: 1px solid #eee">
      &lt;!&ndash;el-aside是左侧标签&ndash;&gt;
      <el-aside width="200px" style="background-color: rgb(238, 241, 246)">
        &lt;!&ndash;左侧菜单内容&ndash;&gt;
       &lt;!&ndash; <el-menu :default-openeds="['1', '3']" :default-active="'1-2'">
          &lt;!&ndash;通过index值来指定默认打开&ndash;&gt;
          <el-submenu index="1">
            &lt;!&ndash;el-submenu 展开菜单栏&ndash;&gt;
            <template slot="title"><i class="el-icon-menu"></i>导航一</template>
            &lt;!&ndash;对于菜单名&ndash;&gt;
              <el-menu-item index="1-1">网关操作</el-menu-item>
              <el-menu-item index="1-2">传感器操作</el-menu-item>
          </el-submenu>&ndash;&gt;
        <el-menu>
          &lt;!&ndash;index代表导航下标&ndash;&gt;
          <el-submenu v-for="(item,index) in $router.options.routes" :index="index+''">
            <template slot="title"><i class="el-icon-menu"></i>{{item.name}}</template>
            <el-menu-item v-for="(item2,index2) in item.children" :index="index+'-'+index2">{{item2.name}}</el-menu-item>
          </el-submenu>
        </el-menu>
      </el-aside>

      <el-container>
        <el-header style="text-align: right; font-size: 12px">
          <el-dropdown>
            <i class="el-icon-setting" style="margin-right: 15px"></i>
            <el-dropdown-menu slot="dropdown">
              <el-dropdown-item>查看</el-dropdown-item>
              <el-dropdown-item>新增</el-dropdown-item>
              <el-dropdown-item>删除</el-dropdown-item>
            </el-dropdown-menu>
          </el-dropdown>
          <span>王小虎</span>
        </el-header>

        <el-main>
          <router-view></router-view>
        </el-main>
      </el-container>
    </el-container>-->
<router-view></router-view>
  </div>

</template>

<style>
  .el-header {
    background-color: #B3C0D1;
    color: #333;
    line-height: 60px;
  }

  .el-aside {
    color: #333;
    height: 100%;
  }
</style>

<script>
    export default {
        data() {
            const item = {
                date: '2016-05-02',
                name: 'deepfeel',
                address: '上海市普陀区金沙江路 1518 弄'
            };
            return {
                tableData: Array(20).fill(item)
            }
        }
    };
</script>
