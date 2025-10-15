<script setup>

</script>

<template>
  <el-container>
      <el-aside width="200px">Aside</el-aside>

      <el-container>
        <el-header>
          <div style="float: left;position: relative;left: 45%">
            <strong>VueManager后台管理系统</strong>
          </div>
          <div class="header-avatar">
            <el-avatar src="https://cube.elemecdn.com/0/88/03b0d39583f48206768a7534e55bcpng.png"></el-avatar>

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
  text-align: center;
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