<template>	
	<div>
	 <el-table
      :data="userList.list"
      style="width: 100%">
      <el-table-column
        prop="date"
        label="日期"
        width="180">
      </el-table-column>
      <el-table-column
        prop="name"
        label="姓名"
        width="180">
      </el-table-column>
      <el-table-column
        prop="address"
        label="地址">
      </el-table-column>
    </el-table>
	</div>	
</template>
<script>
import {mapState} from 'vuex'
export default {
      data() {
        return {
          tableData: []
          //test
        }
      },
      computed:{
        ...mapState(['userList'])
      },
      
    }
</script>
<style>
</style>