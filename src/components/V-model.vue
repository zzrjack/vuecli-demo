<template lang="">
	<div>
		<div>
			<span>用户名：</span>
			<!-- v-model双向数据绑定
        value属性-vue变量   关联在一起
      -->
			<input type="text" v-model="username" />
		</div>
		<div>
			<span>密码：</span>
			<input type="password" v-model="password" />
		</div>
		<div>
			<span>来自于：</span>
			<!-- 下拉菜单绑定在select上 -->
			<select name="" id="" v-model="from">
				<option value="北京市">北京</option>
				<option value="天津市">天津</option>
			</select>
		</div>
		<div>
			<span>复选框：</span>
			<!-- 遇到复选框v-model的变量值为
        非数组-关联的是复选框的checked属性
        数组-关联的是复选框的value属性 -->
			<input type="checkbox" name="" id="" v-model="hobby" value="抽烟" />抽烟
			<input type="checkbox" name="" id="" v-model="hobby" value="喝酒" />喝酒
			<input type="checkbox" name="" id="" v-model="hobby" value="烫头" />烫头
		</div>
		<!-- 单选 -->
		<div>
			<span>性别</span>
			<input type="radio" name="sex" id="" value="男" v-model="gender" />男
			<input type="radio" name="sex" id="" value="女" v-model="gender" />女
		</div>
	</div>
</template>
<script>
	export default {
		data() {
			return {
				username: '',
				password: '',
				from: '',
				hobby: [],
				gender: '',
			};
		},
		methods: {},
	};
</script>
<style lang=""></style>
