<template>
  <el-row class="min-h-screen bg-blue-400">
    <el-col :span="16" class="flex items-center justify-center flex-col ">
      <div class="text-5xl font-bold text-light-50 mb-4">欢迎回来</div>
      <div class=" text-2xl text-gray-200 text-sm">请你别悄悄松开你的梦想，迟早有天它会在你手里发光</div>
    </el-col>
    <el-col :span="8" class="bg-light-50 flex-col flex items-center justify-center">
      <div class="text-lg text-gray-500  font-semibold my-4">账号密码登录</div>
      <el-form size="large" :label-position="labelPosition" :model="formLabelAlign">
        <el-form-item label="账号">
          <el-input v-model="formLabelAlign.name" />
        </el-form-item>
        <el-form-item label="密码">
          <el-input v-model="formLabelAlign.name" />
        </el-form-item>
      </el-form>
      <el-button type="primary" size="large" round>Primary</el-button>
    </el-col>
  </el-row>
</template>

<script setup>
import { reactive, ref } from 'vue'

const labelPosition = ref('right')

const formLabelAlign = reactive({
  name: '',
  region: '',
  type: '',
})
</script>

<style scoped>

</style>
