<template>
	<div>
		<h2>Watch</h2>
		<p>[Conversion between meters and kilometers]</p>
		Kilometer: <input type = "text" v-model = "kilometers">
		Reversed: <input type = "text" v-model = "meters">
	</div>
</template>
<script>
	export default{
		data: {
            kilometers: 0,
            meters: 0
		},
        methods: {
        },
        computed:{
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