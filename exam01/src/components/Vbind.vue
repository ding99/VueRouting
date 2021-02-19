<template>
	<div>
		<h2>V-bind</h2>
		<label for = "r1">change color 1</label>
		<input type = "checkbox" v-model = "use1" id = "r1">
		<br>
		<div v-bind:class = "{'class1': use1 }">v-bind:class directive 1</div>
		<br>

		<label for = "r2">change color 2</label>
		<input type = "checkbox" v-model = "use2" id = "r2">
		<br>
		<div v-bind:class = "{'class2': use2 }">v-bind:class directive 2</div>
	</div>
</template>

<script>
	var data = {use2: false}
	export default{
		data: {use1: false}
	}
</script>

<style>
	.class1 { background: #444; color: rgba(248, 244, 3, 0.89); }
	.class2 { background: rgb(41, 3, 156); color: rgba(238, 243, 236, 0.89); }
</style>