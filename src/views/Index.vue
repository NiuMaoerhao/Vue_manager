<script setup>

</script>

<template>
  <el-container>
      <el-aside width="200px">
        <el-menu
            default-active="2"
            class="el-menu-vertical-demo"
            @open="handleOpen"
            @close="handleClose"
            background-color="#545c64"
            text-color="#fff"
            active-text-color="#ffd04b">
          <el-submenu index="1">
            <template slot="title">
              <i class="el-icon-location"></i>
              <span>导航一</span>
            </template>
            <el-menu-item-group>
              <template slot="title">分组一</template>
              <el-menu-item index="1-1">选项1</el-menu-item>
              <el-menu-item index="1-2">选项2</el-menu-item>
            </el-menu-item-group>
            <el-menu-item-group title="分组2">
              <el-menu-item index="1-3">选项3</el-menu-item>
            </el-menu-item-group>
            <el-submenu index="1-4">
              <template slot="title">选项4</template>
              <el-menu-item index="1-4-1">选项1</el-menu-item>
            </el-submenu>
          </el-submenu>
          <el-menu-item index="2">
            <i class="el-icon-menu"></i>
            <span slot="title">导航二</span>
          </el-menu-item>
          <el-menu-item index="3" disabled>
            <i class="el-icon-document"></i>
            <span slot="title">导航三</span>
          </el-menu-item>
          <el-menu-item index="4">
            <i class="el-icon-setting"></i>
            <span slot="title">导航四</span>
          </el-menu-item>
        </el-menu>

      </el-aside>

      <el-container>
        <el-header>
          <div style="float: left;position: relative;left: 45%">
            <strong>VueManager后台管理系统</strong>
          </div>
          <div class="header-avatar">
            <el-avatar :src="require('@/assets/user.jpg')"></el-avatar>

            <el-dropdown>
                  <span class="el-dropdown-link">
                      Admin<i class="el-icon-arrow-down el-icon--right"></i>
                  </span>
                  <el-dropdown-menu slot="dropdown">
                      <el-dropdown-item>个人中心</el-dropdown-item>
                      <el-dropdown-item>退出</el-dropdown-item>
                  </el-dropdown-menu>
            </el-dropdown>
          </div>

        </el-header>

      <el-main>Main</el-main>
    </el-container>
  </el-container>
</template>

<script>
    export default {
        name: "Index"
    }
</script>


<style scoped>
.el-container {
  padding: 0;
  margin: 0;
  display: flex;
  min-height: 100vh;
}

.el-header {
  background-color: #17B3A3;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 20px;
  height: 60px;
}


.header-avatar {
  display: flex;
  align-items: center;
  gap: 10px;
}


.el-dropdown-link {
  display: flex;
  align-items: center;
  cursor: pointer;
}


.el-aside {
  background-color: #D3DCE6;
  color: #333;
  text-align: left;
  line-height: 200px;
}

.el-main {
  color: #333;
  text-align: center;
  line-height: 160px;
  padding: 0;
}


.el-menu-vertical-demo {
  height: 100%;
}

a {
  text-decoration: none;
}

</style>