<template>
	<div id="app">
		<div class="circle-img-container" style="height: 300px;width: 400px;">
			<div class="circle-img" style="border-radius: 200px;">
				<img src="./assets/Blue_Steel.jpg">
			</div>
		</div>
		<router-view/>
	</div>
</template>

<script>
export default {
	name: 'App'
};
</script>

<style>
#app {
	font-family: "Avenir", Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}

.circle-img-container {
    display: block;
    margin-right: auto;
    margin-left: auto;
}

.circle-img {
    width: 100%;
    height: 100%;
    border-radius: 50%;
    position: relative;
    overflow: hidden;
}

.circle-img img {
    width: 100%;
    height: 100%;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
}
</style>
