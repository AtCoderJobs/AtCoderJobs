<template>
  <el-container>
    <el-header height="56px">
      <h1>AtCoderJobs</h1>
      <el-button type="text">ログイン</el-button>
    </el-header>
    <el-container>
      <el-aside width="256px">
        <el-form @submit.native.prevent>
          <el-form-item label="AtCoderランク">
            <el-checkbox-group v-model="checkList">
              <el-checkbox label="RED"></el-checkbox>
              <el-checkbox label="YELLOW"></el-checkbox>
              <el-checkbox label="BLUE"></el-checkbox>
              <el-checkbox label="GREEN"></el-checkbox>
              <el-checkbox label="GREY"></el-checkbox>
            </el-checkbox-group>
          </el-form-item>
          <el-form-item label="職種"></el-form-item>
          <el-form-item label="勤務地"></el-form-item>
        </el-form>
        <a href="https://github.com/AtCoderJobs/AtCoderJobs" target="_blank" style="text-align: center">View on GitHub</a>
      </el-aside>
      <el-main>
        <el-card>
          <img src="/images/1.jpg" alt="そら">
        </el-card>
        <el-card>
          <img src="/images/2.jpg" alt="あき">
        </el-card>
        <el-card>
          <img src="/images/3.jpg" alt="もり">
        </el-card>
        <el-card>
          <img src="/images/4.jpg" alt="はな">
        </el-card>
        <el-card>
          <img src="/images/5.jpg" alt="はな">
        </el-card>
        <el-card>
          <img src="/images/6.jpg" alt="やま">
        </el-card>
        <el-card>
          <img src="/images/7.jpg" alt="うま">
        </el-card>
        <el-card>
          <img src="/images/8.jpg" alt="すな">
        </el-card>
      </el-main>
    </el-container>
  </el-container>
</template>

<script>
  export default {
    data() {
      return {
        checkList: ['RED', 'YELLOW']
      };
    }
  }
</script>

<style>
  .el-header {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: #FFFFFF;
    background-color: #3F51B5;
  }

  .el-button {
    color: #FFFFFF;
  }

  .el-aside {
    position: fixed;
    top: 56px;
    bottom: 0;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 8px 0;
    background-color: #FAFAFA;
    box-shadow: inset -2px 0 0 #E5E5E5;
  }

  .el-form-item__label {
    float: none;
    margin-left: 16px;
  }

  .el-checkbox-group {
    display: flex;
    flex-direction: column;
  }

  .el-checkbox {
    margin-left: 32px;
  }

  .el-main {
    padding: 56px 0 0 256px;
  }

  .el-card {
    margin: 16px;
    height: 128px;
  }

  .el-card__body {
    padding: 0;
  }
</style>
