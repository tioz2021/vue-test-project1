<template>
	<div class="wrp">
		<ul>
			<li>1</li>
			<li>2</li>
			<li>3</li>
			<li>4</li>
			<li>5</li>
		</ul>
	</div>
	<button @click="handleClick">Move</button>
</template>
<script>
	export default {
		name: 'MySlider', 
		methods: {
			handleClick() {
				document.querySelector('ul').style.transform = 'translateX(-50%)'
			}
		}
	}
</script>

<style>
 .wrp{
	width: 500px;
	border: 1px dashed green;
 }
	ul{
		display: flex;
		flex-direction: row;
		padding: 0;
		margin: 0;
		width: 200%;
		list-style: none;
		transform: translateX('0');
		transition: all 1000ms ease;
	}
	li{
		width: 33%;
		border: 1px solid red;
	}
</style>