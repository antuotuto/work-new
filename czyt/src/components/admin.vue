<template>
<!--  -->
<div class="admin">
  <crumbs></crumbs>

  <el-tabs type="border-card">
    <el-tab-pane>
      <span slot="label">
        <i class="el-icon-search"></i> 查找</span>
        <excl></excl>
    </el-tab-pane>
    <el-tab-pane>
      <span slot="label">
        <i class="el-icon-plus"></i> 新增</span>
        <excl></excl>
    </el-tab-pane>
  </el-tabs>

  <paging></paging>

</div>
<!--  -->
</template>

<script>
import excl from '~/components/excl.vue'
import crumbs from '~/components/crumbs.vue'
import paging from '~/components/paging.vue'

export default {
  components: {
    excl,
    crumbs,
    paging
  },
  data() {
    return {}
  },
  watch: {},
  methods: {

  },
  directives: {},
  created() {},
  mounted() {}
}
</script>

<style scoped>


</style>
