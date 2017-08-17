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


      <el-row :gutter="20">
        <el-col :span="12" :offset="6">
          <div class="grid-content bg-purple">
            <el-form :label-position="labelPosition" label-width="80px" :model="formLabelAlign">
              <el-form-item label="名称 :">
                <el-input v-model="formLabelAlign.name"></el-input>
              </el-form-item>
              <el-form-item label="活动区域 :">
                <el-input v-model="formLabelAlign.region"></el-input>
              </el-form-item>
              <el-form-item label="活动形式 :">
                <el-input v-model="formLabelAlign.type"></el-input>
              </el-form-item>
              <el-form-item label="活动地点 :">
                <el-input v-model="formLabelAlign.type"></el-input>
              </el-form-item>
            </el-form>
          </div>
        </el-col>
        <el-col :span="6">
          <div class="grid-content bg-purple"></div>
        </el-col>
      </el-row>

      <el-row>
        <el-col :span="12" :offset="6">
          <div class="button-on">
            <el-button type="primary">提交修改</el-button>
          </div>
        </el-col>
        <el-col :span="6">
          <div class="grid-content bg-purple-light"></div>
        </el-col>
      </el-row>


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
    return {
      labelPosition: 'top',
      formLabelAlign: {
        name: '',
        region: '',
        type: ''
      }
    }
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
.el-row {
  margin-bottom: 15px;
}
.button-on{
  padding-left: 5px;
}
</style>
