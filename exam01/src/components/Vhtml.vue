<template>
	<div>
		<h2>v-html</h2>
		<p>{{ message }}</p>
        <div v-html = "message"></div>
	</div>
</template>

<script>
	export default{
		data: function() {
			return {
				message: '<h4>Hello, v-html directive!</h4>'
			}
		}
	}
</script>