<template>
  <el-container class="home-container">
    <!-- 管理菜单头部 -->
    <el-header>
      <Header />
    </el-header>
    <!-- 内容区域 -->
    <el-container>
      <el-aside width="270px">
        <Menu />
      </el-aside>
      <el-container>
        <el-main>
          <Main />
        </el-main>
        <el-footer>
          <Footer />
        </el-footer>
      </el-container>
    </el-container>
  </el-container>
</template>

<script>
import Menu from "@/components/sys/Menu";
import Footer from "@/components/sys/Footer";
import Main from "@/components/sys/Main";
import Header from "@/components/sys/Header";

export default {
  name: "AppIndex",
  components: {
    Menu,
    Footer,
    Main,
    Header
  }
};
</script>

<style scoped>
.home-container {
  height: 100%;
}
.el-header {
  background-color: #f0f9eb;
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 20px;
}
.el-footer {
  background-color: antiquewhite;
  color: #333;
  text-align: left;
  line-height: 60px;
}

.el-aside {
  color: #333;
  line-height: 200px;
  background-color: white;
  text-align: left;
  padding: 10px;
}
</style>
