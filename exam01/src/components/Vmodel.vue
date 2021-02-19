<template>
	<div>
		<h2>v-model</h2>
		<p>{{ message }}</p>
        <input v-model = "message">
	</div>
</template>

<script>
	export default{
		data: function() {
			return {
				message: 'Beginning'
			}
		}
    }
</script>