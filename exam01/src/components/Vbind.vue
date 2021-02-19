<template>
	<div>
		<h2>V-bind</h2>
		<label for = "r1">change color</label>
		<input type = "checkbox" v-model = "use" id = "r1">
		<br>
		<div v-bind:class = "{'class1': use }">v-bind:class directive</div>
	</div>
</template>

<script>
	//export default{
	var	data = {use: false}
	//}
</script>

<style>
	.class1 {
		background: #444;
		color: rgba(248, 244, 3, 0.89);
	}
</style>