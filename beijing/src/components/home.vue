<template>
<div class="home">
  <div class="home-left">
    <leftMenu></leftMenu>
  </div>
  <div class="home-right">
    <router-view></router-view>
  </div>
</div>
</template>

<script>
import leftMenu from '~/components/leftMenu.vue'

export default {
  name: 'home',
  data() {
    return {

    }
  },
  components: {
    leftMenu
  },
  methods: {

  },
  watch: {},
  created() {},
}
</script>

<style scoped lang="scss">
.home {
    height: 100%;
}
.home-left {
    float: left;
    width: 200px;
    height: 100%;
    background: #324157;
}
.home-right {
    overflow: hidden;
    padding: 15px;
}

::-webkit-scrollbar-track-piece {
    background-color: rgba(0, 0, 0, 0);
    border-radius: 0;
}
</style>
