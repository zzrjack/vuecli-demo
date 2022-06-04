<template>
	<div>
		<!-- 语法:
      :class="{类名: 布尔值}"
      使用场景: vue变量控制标签是否应该有类名
     -->
		<p :class="{ red_str: bool }">动态class</p>
		<p :style="{ backgroundColor: colorStr }">动态style</p>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				bool: true,
				colorStr: 'red',
			};
		},
	};
</script>

<style scoped>
	.red_str {
		color: blue;
	}
</style>
