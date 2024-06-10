<script setup>
	import {RouterView, RouterLink} from 'vue-router'
</script>

<template>
	<main>
		<div class='links'>
			<RouterLink active-class='active' to='/' class="btn">Home</RouterLink>
			<RouterLink active-class='active' to='/about' class="btn">About</RouterLink>
			<RouterLink active-class='active' to='/GA' class="btn">GA</RouterLink>
		</div>
		<RouterView />
	</main>
</template>

<style scoped>
	.links {
		padding: 20px
	}
	.links a {
		margin: 0 5px
	}
	/* .active {
		font-weight: bold;
		color: green;
	} */
	main{
		background-color: rgb(209, 254, 254);
	}
	#links {
    text-align: center;
    margin-bottom:-50px;
	}
	.btn{
		display:inline;
		background-color: rgb(124, 158, 239);
		border-radius:25px;
		padding: 9px;
		color:white;
		text-decoration: none;
		cursor: pointer; 
		transition: color 0.3s ease, background-color 0.3s ease; 
	}
	.btn:hover{
		font-weight: bold;
		background-color: rgb(242, 197, 231);
		color: rgb(95, 137, 181);
	}
</style>