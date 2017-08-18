<template>
<div id="app">
  <header>
    <p>海南残联管理系统</p>
    <el-col class="navbar">
      <el-menu theme="light" default-active="1" mode="horizontal" :router="true">
        <el-menu-item index="1" :route="{path:'/home'}">个性化服务系统</el-menu-item>
        <el-menu-item index="2" :route="{path:'/excl'}">基金会系统</el-menu-item>
        <el-menu-item index="3" :route="{path:'/excl1'}">资金管理系统</el-menu-item>
        <el-menu-item index="4" :route="{path:'/excl1'}">志愿者服务系统</el-menu-item>
        <el-menu-item index="5" :route="{path:'/excl1'}">基础平台系统</el-menu-item>
      </el-menu>
    </el-col>
  </header>
  <main>
    <router-view></router-view>
  </main>
</div>
</template>

<script>
export default {
  data() {
    return {}
  },
  methods: {

  },
  components: {}
}
</script>

<style lang="scss">
#app {
    font-family: Helvetica, sans-serif;
    height: 100%;
    background: #eef1f6;
}

header {
    height: 60px;
    padding-left: 200px;
    position: relative;
    z-index: 1000;
    p {
        position: absolute;
        top: 0;
        left: 0;
        width: 200px;
        height: 60px;
        line-height: 60px;
        text-align: center;
        background: #324157;
        color: #fff;
        font-weight: bold;
        font-size: 18px;
    }
    .el-menu {
        background: #fff;
    }
}

main {
    height: 100%;
    width: 100%;
    position: absolute;
    top: 0;
    left: 0;
    padding-top: 60px;
    box-sizing: border-box;
}

.navbar .el-menu-item.is-active {
    border-bottom: 5px solid #20a0ff;
    background-color: #eef1f6;
}

::-webkit-scrollbar {
    width: 4px;
    background: rgba(0, 0, 0, 0.08);
}

::-webkit-scrollbar-thumb {
    background: #a4a4a4;
    border-radius: 0;
}
</style>
