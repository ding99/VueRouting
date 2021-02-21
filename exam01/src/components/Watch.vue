<template>
	<div>
		<h2>Compute</h2>
		<p>[reverse the string]</p>
		<p>Original: {{ message }}</p>
		<p>Reversed: {{ messageMsg }}</p>
        <input v-model = "message">
	</div>
</template>

<script>
	export default{
		data: function() {
			return {
				message: 'Computing'
			}
		},
		computed: {
            messageMsg: function() {
			    return this.message.split('').reverse().join('')
            }
        }
    }
</script>