<template>
    <div>
        <div class="card">
            <!-- v-model 数据的双向绑定 页面值改变，变量值也改变 -->
            <!-- v-bind 单向绑定页面改了数据不会变，简写为： 这里的refix-icon 是input的属性表示左侧显示Search图标-->
            <el-input style="width: 300px;" v-model="data.name" placeholder="请输入名称查询" :prefix-icon="Search"/>
            <!-- @ 是v-on的简写，表示绑定事件函数 -->
            <el-button @click="load" type="primary" style="margin-left: 12px;">查询</el-button>
            <el-button @click="reset" type="info">重置</el-button>
        </div>
    </div>
</template>

<script setup>
import { reactive } from 'vue';
// @element-plus/icons-vue 在package.json里面有安装过 
import { Search } from "@element-plus/icons-vue"

// reactive 建立交互式对象
const data = reactive({
    name: null
})

// 分页查询数据的函数
const load = () => {

}

const reset = () => {

}
</script>