<template>
	<div>
		<h2>v-model</h2>
		<p>{{ message }}</p>
        <input v-model = "message">
	</div>
</template>

<script>
	export default{
	    data:{message:'Beginning'}
	}
</script>