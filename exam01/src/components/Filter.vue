<template>
	<div>
		<h2>Filter</h2>
		<p>[Change the first letter to upper-case]</p>
		<p>Original: {{ message }}</p>
		<p>Filtered: {{ message | capi }}</p>
        <input v-model = "message">
	</div>
</template>

<script>
	export default{
		data: function() {
			return {
				message: 'modify'
			}
		},
		filters: {
            capi: function(value) {
                if(!value) return ''
                value = value.toString()
			    return value.charAt(0).toUpperCase() + value.slice(1)
            }
        }
    }
</script>