<template>
	<div>
		<h2>Watch</h2>
		<p>[Conversion between meters and kilometers]</p>
		Kilometers: <input type = "text" v-model = "kilometers">
		Meters: <input type = "text" v-model = "meters">
	</div>
</template>
<script>
	export default{
		data: function() {
            return {
                kilometers: 0,
                meters: 0
            }
		},
		watch: {
            kilometers: function(val){
                this.kilometers = val;
                this.meters = val * 1000
            },
            meters: function(val) {
                this.kilometers = val / 1000;
                this.meters = val
            }
        }
    }
</script>