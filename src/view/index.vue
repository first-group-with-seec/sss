<template>
    <div>
        <div class="content">
            <topBox></topBox>
            <logo></logo>
            <div class="list">
                <el-container style="height: 500px; border: 1px solid #eee">
                    <el-aside width="200px" style="background-color: rgb(238, 241, 246)">
                        <div class="tit">
                            大路平台
                        </div>
                        <el-menu :default-openeds="['1', '3']">
                        <el-submenu index="0">
                            <template slot="title">用户管理</template>
                        </el-submenu>
                        <el-submenu index="1">
                            <template slot="title">角色管理</template>
                        </el-submenu>
                        <el-submenu index="2">
                            <template slot="title">账户管理</template>
                            <el-menu-item-group>
                            <el-menu-item index="2-1">创建子账户</el-menu-item>
                            <el-menu-item index="2-2">管理子账户</el-menu-item>
                            </el-menu-item-group>
                        </el-submenu>
                        <el-submenu index="3">
                            <template slot="title">利率设置</template>
                        </el-submenu>
                        <el-submenu index="4">
                            <template slot="title">财务部门审核</template>
                            <el-menu-item-group>
                            <el-menu-item index="4-1">放款审核</el-menu-item>
                            <el-menu-item index="4-2">还款确认</el-menu-item>
                            </el-menu-item-group>
                        </el-submenu>
                        <el-submenu index="5">
                            <template slot="title">外综服企业</template>
                            <el-menu-item-group>
                            <el-menu-item index="5-1">企业信息</el-menu-item>
                            <el-menu-item index="5-2">退税融资申请</el-menu-item>
                            <el-menu-item index="5-2">结汇融资申请</el-menu-item>
                            <el-menu-item index="5-2">退税融资申请</el-menu-item>
                            <el-menu-item index="5-2">退税融资申请</el-menu-item>
                            </el-menu-item-group>
                        </el-submenu>
                        <el-submenu index="6">
                            <template slot="title">财务部门审核</template>
                            <el-menu-item-group>
                            <el-menu-item index="6-1">放款审核</el-menu-item>
                            <el-menu-item index="6-2">还款确认</el-menu-item>
                            </el-menu-item-group>
                        </el-submenu>
                        <el-submenu index="7">
                            <template slot="title">财务部门审核</template>
                            <el-menu-item-group>
                            <el-menu-item index="7-1">放款审核</el-menu-item>
                            <el-menu-item index="7-2">还款确认</el-menu-item>
                            </el-menu-item-group>
                        </el-submenu>
                        </el-menu>
                    </el-aside>
                    
                    <el-container>
                        <el-header style="text-align: right; font-size: 12px">
                        <el-dropdown>
                            <i class="el-icon-setting" style="margin-right: 15px"></i>
                            <el-dropdown-menu slot="dropdown">
                            <el-dropdown-item>查看</el-dropdown-item>
                            <el-dropdown-item>新增</el-dropdown-item>
                            <el-dropdown-item>删除</el-dropdown-item>
                            </el-dropdown-menu>
                        </el-dropdown>
                        <span>王小虎</span>
                        </el-header>
                        
                        <el-main>
                        <el-table :data="tableData">
                            <el-table-column prop="date" label="日期" width="140">
                            </el-table-column>
                            <el-table-column prop="name" label="姓名" width="120">
                            </el-table-column>
                            <el-table-column prop="address" label="地址">
                            </el-table-column>
                        </el-table>
                        </el-main>
                    </el-container>
                </el-container>
            </div>
        </div>
    </div>
</template>
<script>
import topBox from '@/components/base/topBox'
import logo from '@/components/base/logo'
export default {
    components:{
        topBox,
        logo
    },
    data() {
      const item = {
        date: '2016-05-02',
        name: '王小虎',
        address: '上海市普陀区金沙江路 1518 弄'
      };
      return {
        tableData: Array(20).fill(item)
      }
    }
}
</script>
<style lang="scss" scoped>
    .el-header {
        background-color: #B3C0D1;
        color: #333;
        line-height: 60px;
    }

    .el-aside {
        color: #333;
    }
    .content{
        .tit{
            background: rgb(115,85,128);
            height:55px;
            color:#fff;
            font-size: 24px;
            line-height: 55px;
            text-align: center;
            margin-bottom:10px;
        }
    }
</style>