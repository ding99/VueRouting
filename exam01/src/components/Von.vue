<template>
	<div>
		<h2>v-on</h2>
		<p>{{ message }}</p>
        <button v-on:click = "reverseMsg">Reverse String</button>
	</div>
</template>

<script>
	export default{
		data: function() {
			return {
				message: 'Beginning'
			}
		},
		methods: {
            reverseMsg: function() {
			    this.message = this.message.split('').reverse().join('')
            }
        }
    }
</script>