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
				message: '<h3>Hello, v-html directive!</h3>'
			}
		}
	}
</script>