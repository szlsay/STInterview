<template>
	<view>
		<!-- 传入符合 datacom 规范的数据，即可渲染出一个选择器  -->
		<!-- 使用 v-model 双向绑定 picker 的选中值 -->
		<uni-data-picker v-model="value" :localdata="items"></uni-data-picker>
	</view>
</template>


<script>
	export default {
		data() {
			return {
				value: ["110000", "110105"],
				items: [{
					"value": "110000",
					"text": "北京市",
					"children": [{
						"value": "110105",
						"text": "朝阳区"
					}, {
						"value": "110108",
						"text": "海淀区"
					}]
				}],
			};
		},
	};
</script>


<style>

</style>