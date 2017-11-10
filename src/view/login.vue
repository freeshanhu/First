<template>
	<div class="login-panel">
	    <p class="login-title">First后台管理系统</p>
	    <el-card class='login-form'>
	        <el-form ref="login" :model="user">
	            <el-form-item>
	                <el-input placeholder='用户名' v-model='user.userName'></el-input>
	            </el-form-item>
	            <el-form-item>
	                <el-input placeholder='密码' v-model='user.password'></el-input>
	            </el-form-item>
	            <el-form-item>
	                <el-button type="primary" class='submit-btn'>登陆</el-button>
	            </el-form-item>
	        </el-form>
	    </el-card>
	</div>
</template>
<script>
	export default {
        data(){
            return {
                user:{
                    userName:null,
                    password:null
                }
            }
        }
    }
</script>
<style lang="less" rel="stylesheet/less">
    .login-panel{
        width: 100%;
        height: 100%;
        padding-top: 200px;
        background: #324057;
        .login-form{
            width: 460px;
            margin: auto;
            padding: 30px;
            .submit-btn{
                width: 400px;
                display: block;
                margin: auto;
            }
        }
        .login-title{
            text-align: center;
            height: 80px;
            line-height: 80px;
            font-size: 48px;
            color: #fff;
        }
    }
</style>