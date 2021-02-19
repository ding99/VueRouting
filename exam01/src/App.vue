<template>
	<div id="app">
		<div class="row">
			<div class="col-xs-offset-2 col-xs-8">
				<div class="page-header">
					<h1>Basic Syntax</h1>
				</div>
			</div>
		</div>
		<div class="row">
			<div class="col-xs-2 col-xs-offset-2">
				<div class="list-group">
					<!-- navigated by v-link -->
					<a class="list-group-item" v-link="{ path: '/home'}">Home</a>
					<a class="list-group-item" v-link="{ path: '/about'}">About</a>
					<a class="list-group-item" v-link="{ path: '/vhtml'}">V-html</a>
					<a class="list-group-item" v-link="{ path: '/vbind'}">V-bind</a>
					<a class="list-group-item" v-link="{ path: '/vmodel'}">V-model</a>
					<a class="list-group-item" v-link="{ path: '/von'}">V-on</a>
				</div>
			</div>
			<div class="col-xs-6">
				<div class="panel">
					<div class="panel-body">
						<!-- render matched components -->
						<router-view></router-view>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<style>
	body {
		background-color: #dfebf7;
	}
</style>